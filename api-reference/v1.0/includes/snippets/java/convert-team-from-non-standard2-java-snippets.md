---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8e7e92a9e73cb2c91e7ddd803a0728ef342203f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984168"
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
ChannelCollectionResponse channelCollectionResponse = new ChannelCollectionResponse();
channelCollectionResponse.value = channelsList;
ChannelCollectionPage channelCollectionPage = new ChannelCollectionPage(channelCollectionResponse, null);
team.channels = channelCollectionPage;
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
TeamsAppInstallationCollectionResponse teamsAppInstallationCollectionResponse = new TeamsAppInstallationCollectionResponse();
teamsAppInstallationCollectionResponse.value = installedAppsList;
TeamsAppInstallationCollectionPage teamsAppInstallationCollectionPage = new TeamsAppInstallationCollectionPage(teamsAppInstallationCollectionResponse, null);
team.installedApps = teamsAppInstallationCollectionPage;

graphClient.teams()
    .buildRequest()
    .post(team);

```