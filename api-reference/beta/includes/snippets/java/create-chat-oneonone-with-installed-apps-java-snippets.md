---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1431b454f42e18a7b5addef151199ed743e2ea748c075497f63d4c1cfd8d376f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278429"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = new Chat();
chat.chatType = ChatType.ONE_ON_ONE;
LinkedList<ConversationMember> membersList = new LinkedList<ConversationMember>();
AadUserConversationMember members = new AadUserConversationMember();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("owner");
members.roles = rolesList;
members.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"));
membersList.add(members);
AadUserConversationMember members1 = new AadUserConversationMember();
LinkedList<String> rolesList1 = new LinkedList<String>();
rolesList1.add("owner");
members1.roles = rolesList1;
members1.additionalDataManager().put("user@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"));
membersList.add(members1);
ConversationMemberCollectionResponse conversationMemberCollectionResponse = new ConversationMemberCollectionResponse();
conversationMemberCollectionResponse.value = membersList;
ConversationMemberCollectionPage conversationMemberCollectionPage = new ConversationMemberCollectionPage(conversationMemberCollectionResponse, null);
chat.members = conversationMemberCollectionPage;
LinkedList<TeamsAppInstallation> installedAppsList = new LinkedList<TeamsAppInstallation>();
TeamsAppInstallation installedApps = new TeamsAppInstallation();
installedApps.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/appCatalogs/teamsApps/05F59CEC-A742-4A50-A62E-202A57E478A4"));
installedAppsList.add(installedApps);
TeamsAppInstallationCollectionResponse teamsAppInstallationCollectionResponse = new TeamsAppInstallationCollectionResponse();
teamsAppInstallationCollectionResponse.value = installedAppsList;
TeamsAppInstallationCollectionPage teamsAppInstallationCollectionPage = new TeamsAppInstallationCollectionPage(teamsAppInstallationCollectionResponse, null);
chat.installedApps = teamsAppInstallationCollectionPage;

graphClient.chats()
    .buildRequest()
    .post(chat);

```