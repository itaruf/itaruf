### Welcome to my world ~ 👋
```
#include "contacts.h"
#include "hobbies.h"
#include "languages.h"
#include "profile.h"
#include "softwares.h"

int main() 
{
  Profile profile;
  profile.set_name("Imane Taruf");
  profile.set_title("Junior Game Programmer");
  profile.add_education("IIM Digital School", "Master's Degree in Gamme Programming", 2021, 2023);
  profile.add_education("Paris Cite University", "Bachelor's Degree in Computer Science", 2018, 2021);
  profile.add_soft({"Communication", "Creativity", "Problem-Solving", "Teamwork", "Collaboration", "Adaptabiltity", "Curious"});

  Contacts contacts;
  contacts.set_email("imane.taruf@gmail.com");
  contacts.set_linkedin("https://www.linkedin.com/in/imane-taruf-53040320a/");

  Language languages;
  languages.add_programming({"C", "C++", "C#", "Python"});
  languages.add_computer({"HTML", "CSS", "JSON"});
  languages.add_scripting("Unreal Engine's Blueprints");
  languages.add_real({"French: Native", "English: Fluent", "Japanese: Beginner", "Spanish: Beginner"});

  Software softwares;
  softwares.add_game_engine({"Unreal Engine 4", "Unreal Engine 5", "Unity", "Ubisoft's Anvil"});
  softwares.add_ide({"Visual Studio Code", "Visual Studio Community 2019/2022", "JetBrains Rider", "JetBrains Python", "Eclipse"});
  softwares.add_version_control({"Git", "Perforce"});
  
  Hobbies hobbies;
  hobbies.add({"Video Games", "Retrograming", "Game development", "Game Jams", "Japanese Culture", "eSports"});

  return 0;
}
