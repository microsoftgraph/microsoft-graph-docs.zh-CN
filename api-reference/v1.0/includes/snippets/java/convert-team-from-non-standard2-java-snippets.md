---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 521f73ef92844ffcfc414b94694886ecd8db8a34
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374054"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.additionalDataManager().put("template@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')"));
team.displayName = "My Class Team";
team.description = "My Class Team’s Description";
LinkedList<Channel> channelsList = new LinkedList<Channel>();
Channel channels = new Channel();
channels.displayName = "Class Announcements 📢";
channels.isFavoriteByDefault = true;
channelsList.add(channels);
Channel channels1 = new Channel();
channels1.displayName = "Homework 🏋️";
channels1.isFavoriteByDefault = true;
channelsList.add(channels1);
team.channels = channelsList;
TeamMemberSettings memberSettings = new TeamMemberSettings();
memberSettings.allowCreateUpdateChannels = false;
memberSettings.allowDeleteChannels = false;
memberSettings.allowAddRemoveApps = false;
memberSettings.allowCreateUpdateRemoveTabs = false;
memberSettings.allowCreateUpdateRemoveConnectors = false;
team.memberSettings = memberSettings;
LinkedList<TeamsAppInstallation> installedAppsList = new LinkedList<TeamsAppInstallation>();
TeamsAppInstallation installedApps = new TeamsAppInstallation();
installedApps.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"));
installedAppsList.add(installedApps);
TeamsAppInstallation installedApps1 = new TeamsAppInstallation();
installedApps1.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"));
installedAppsList.add(installedApps1);
team.installedApps = installedAppsList;

graphClient.teams()
    .buildRequest()
    .post(team);

```