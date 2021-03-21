---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5631b33a661ac7df7ba7490f879740781b7f83f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960022"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsTab teamsTab = new TeamsTab();
teamsTab.displayName = "My Contoso Tab";
teamsTab.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8"));
TeamsTabConfiguration configuration = new TeamsTabConfiguration();
configuration.entityId = "2DCA2E6C7A10415CAF6B8AB6661B3154";
configuration.contentUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView";
configuration.websiteUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154";
configuration.removeUrl = "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab";
teamsTab.configuration = configuration;

graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").tabs()
    .buildRequest()
    .post(teamsTab);

```