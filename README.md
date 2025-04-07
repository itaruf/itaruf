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
    experience.add("CNRS-AIST JRL, Tsukuba, Japan", "XR & Game Technologies Engineer | Humanoid-Robot Teleoperation", "09/2024", "Present", {
        "In charge of developing systems for humanoid-robot teleoperation using XR and game technologies to build the most immersive experience possible.",
        "• Designed extensible systems for humanoid-robot teleoperation using XR and game technologies",
        "• Integrated third-party SDKs to expand interaction capabilities and device options for users",
        "• Migrated the VR system to OpenXR for long-term support and cross-platform compatibility",
        "• Developed custom editor tools to manage system data and streamline development and debugging",
        "• Configured projects for standalone optimized builds to support future-ready distributions",
        "• Established CI/CD pipelines to support scheduled releases and track stages (e.g., public showcases)",
        "• Authored technical documentation to support onboarding and team collaboration"
    });

    experience.add("Ubisoft Bordeaux, France", "Gameplay Programmer Intern", "02/2023", "08/2023", {
        "Collaborated within an international game development team of 6 developers to enhance AI systems",
        "Worked on Assassin’s Creed Mirage, a AAA game with over 5M copies sold in 4 months of release",
        "Developed real-time gameplay features in C++ for AI navigation, decision-making, and entity detection",
        "Worked using Visual Studio 2022, and Anvil Engine, a C++ game engine codebase of 10M lines",
        "Troubleshot issues and tested developed solutions, ensuring quality for various in-game scenarios",
        "Used Perforce for version control, and Helix Swarm for code reviews to maintain best practices"
    });

    Languages languages;
    languages.add_programming({ "C", "C++", "C#", "Python" });
    languages.add_computer({ "HTML", "CSS", "JSON", "JavaScript" });
    languages.add_scripting("Unreal Engine's Blueprints");
    languages.add_real({ "French: Native", "English: Business Level", "Japanese: Low Intermediate"});

    Softwares softwares;
    softwares.add_game_engine({ "Unreal Engine 4", "Unreal Engine 5", "Unity", "Ubisoft’s Anvil" });
    softwares.add_ide({ "Visual Studio Code", "Visual Studio Community 2019/2022", "JetBrains Rider", "JetBrains PyCharm", "Eclipse" });
    softwares.add_version_control({ "Git", "Perforce" });
    softwares.add_collaboration_tools({ "Jira", "Confluence", "Microsoft 365", "Slack", "Notion", "Trello", "Miro" });

    Hobbies hobbies;
    hobbies.add({ "Video Games", "Retrograming", "Game development", "Game Jams", "Japanese Culture", "Anime", "Manga", "eSports" });

    return 0;
}
