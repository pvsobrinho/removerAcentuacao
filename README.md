Remover acentuação em Java, exceto ponto (.)

private static String removeNonASCIIChars(String query) {
        return Normalizer.normalize(query, Normalizer.Form.NFD)
                .replaceAll("[^\\p{ASCII}]", "");
    }
