System.out.println("\nCurrent Time");

if (locale.equals(Locale.US)) {

    System.out.println("USA : "
            + ZonedDateTime.now(ZoneId.of("America/New_York"))
                    .format(formatter));

}
else if (locale.getLanguage().equals("hi")) {

    System.out.println("India : "
            + ZonedDateTime.now(ZoneId.of("Asia/Kolkata"))
                    .format(formatter));

}
else if (locale.equals(Locale.FRANCE)) {

    System.out.println("France : "
            + ZonedDateTime.now(ZoneId.of("Europe/Paris"))
                    .format(formatter));

}
