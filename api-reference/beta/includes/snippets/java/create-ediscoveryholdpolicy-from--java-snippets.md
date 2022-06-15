---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43f2099fe46053dc26128fc1004311c3677b39be
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096129"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryHoldPolicy ediscoveryHoldPolicy = new EdiscoveryHoldPolicy();
ediscoveryHoldPolicy.displayname = "My legalHold with sources";
ediscoveryHoldPolicy.description = "Created from Graph API";
ediscoveryHoldPolicy.contentQuery = "Bazooka";
ediscoveryHoldPolicy.additionalDataManager().put("userSources@odata.bind", new JsonPrimitive("[  {    \"@odata.type\": \"microsoft.graph.security.userSource\",    \"email\": \"SalesTeam@M365x809305.OnMicrosoft.com\"  }]"));
ediscoveryHoldPolicy.additionalDataManager().put("siteSources@odata.bind", new JsonPrimitive("[  {    \"@odata.type\": \"microsoft.graph.security.siteSource\",    \"site\": {      \"webUrl\": \"https://m365x809305.sharepoint.com/sites/Design-topsecret\"    }  }]"));

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").legalHolds()
    .buildRequest()
    .post(ediscoveryHoldPolicy);

```