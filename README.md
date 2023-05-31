# Anastas Risteski 182065
Control Flow Graph


![CFG1](https://github.com/anastasristeski/SI_2023_lab2_182065/assets/77769395/e116bd0a-7198-4cdb-8560-d5e0867c1e6d)



Цикломатска Коплексност

    Цикломатската комплексност ја пресметав по формулата e-n+2p
      e=33,n=24,p=1;/ 33-24+2=11
        Цикломатската комплексност е 11      

Тест случаи според every branch

Branch 1: if (user==null || user.getPassword()==null || user.getEmail()==null)

Test case 1: user = null, user.getPassword() = null, user.getEmail() = null
Branch 2: if (user.getUsername()==null)

Test case 1: user.getUsername() = null
Test case 2: user.getUsername() != null
Branch 3: if (user.getEmail().contains("@") && user.getEmail().contains("."))

Test case 1: user.getEmail() = null
Test case 2: user.getEmail() does not contain "@"
Test case 3: user.getEmail() does not contain "."
Test case 4: user.getEmail() contains "@" and "."
Branch 4: if (existingUser.getEmail() == user.getEmail())

Test case 1: existingUser.getEmail() = null, user.getEmail() = null
Test case 2: existingUser.getEmail() != user.getEmail()
Branch 5: if (existingUser.getUsername() == user.getUsername())

Test case 1: existingUser.getUsername() = null, user.getUsername() = null
Test case 2: existingUser.getUsername() != user.getUsername()
Branch 6: if (passwordLower.contains(user.getUsername().toLowerCase()) || password.length()<8)

Test case 1: passwordLower contains user.getUsername().toLowerCase(), password.length() < 8
Test case 2: passwordLower contains user.getUsername().toLowerCase(), password.length() >= 8
Test case 3: passwordLower does not contain user.getUsername().toLowerCase(), password.length() < 8
Test case 4: passwordLower does not contain user.getUsername().toLowerCase(), password.length() >= 8
Branch 7: if (!passwordLower.contains(" "))

Test case 1: passwordLower contains " "
Test case 2: passwordLower does not contain " "
Branch 8: if (password.contains(String.valueOf(specialCharacters.charAt(i))))

Test case 1: password does not contain any special characters


Тест случаи според Multiple Condition

Test case 1:

user = null
user.getPassword() = null
user.getEmail() = null
Test case 2:

user = null
user.getPassword() = null
user.getEmail() != null
Test case 3:

user = null
user.getPassword() != null
user.getEmail() = null
Test case 4:

user = null
user.getPassword() != null
user.getEmail() != null
Test case 5:

user != null
user.getPassword() = null
user.getEmail() = null
Test case 6:

user != null
user.getPassword() = null
user.getEmail() != null
Test case 7:

user != null
user.getPassword() != null
user.getEmail() = null
Test case 8:

user != null
user.getPassword() != null
user.getEmail() != null
