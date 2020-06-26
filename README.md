 /* find the frequency of a character*/
 char y[1000], character;
     int count = 0;

     printf("Enter a string: ");
     fgets(y, sizeof(y), stdin);

     printf("Enter a character to find its frequency: ");
     scanf("%c", &character);

     for (int i = 0; y[i] != '\0'; ++i) {
         if (character == y[i])
             ++count;
     }

     printf("Frequency of %c = %d\n", character, count);
     return 0;
