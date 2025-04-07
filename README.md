### Welcome to my world 👋 ~ Start exploring  ~ [now](https://github.com/itaruf?tab=stars) ~ ⭐
```
#include "profile.h"
#include "education.h"
#include "experience.h"
#include "languages.h"
#include "softwares.h"
#include "hobbies.h"

int main()
{
    Profile profile;
    profile.set_name("Imane Taruf");
    profile.set_title("Software Engineer");
    profile.set_email("imane.taruf@gmail.com");

    Education education;
    education.add("IIM Digital School", "Master's Degree in Game Programming", 2021, 2023);
    education.add("University of Paris Cité", "Bachelor's Degree in Computer Science", 2018, 2021);

    Experience experience;
    experience.add("CNRS-AIST JRL, Tsukuba, Japan", "XR & Game Technologies Engineer | Humanoid-Robot", "09/2024", "Present",
    { "In charge of developing systems for humanoid-robot teleoperation using XR and game technologies." });

    experience.add("Ubisoft Bordeaux, France", "Gameplay Programmer Intern", "02/2023", "08/2023",
    { "Worked within an international game development to enhance AI systems for the AAA game Assassin's Creed Mirage." });

    Languages languages;
    languages.add_programming({ "C/C++", "C#", "Python" });
    languages.add_scripting("Unreal Engine's Blueprints");
    languages.add_real({ "French: Native", "English: Business Level", "Japanese: Low Intermediate"});

    Softwares softwares;
    softwares.add_game_engine({ "Unreal Engine 4", "Unreal Engine 5", "Unity", "Ubisoft’s Anvil" });
    softwares.add_ide({ "Visual Studio Code", "Visual Studio Community 2019/2022", "JetBrains Rider" });
    softwares.add_version_control({ "Git", "Perforce" });
    softwares.add_collaboration_tools({ "Jira", "Confluence", "Microsoft 365", "Slack", "Notion", "Trello", "Miro" });

    Hobbies hobbies;
    hobbies.add({ "Video Games", "Retrograming", "Game development", "Game Jams", "Japanese Culture", "Anime", "Manga", "eSports" });

    return 0;
}
