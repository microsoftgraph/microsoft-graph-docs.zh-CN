---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71fed7fac58e710fefc370c062b0b83b4ed9f4b1798075b4f38ebde72b4d9454
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219981"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> hubSiteUrlsList = new LinkedList<String>();
hubSiteUrlsList.add("https://graph.microsoft.com/beta/sites/id");

Boolean propagateToExistingLists = false;

graphClient.sites("id").contentTypes("id")
    .associateWithHubSites(ContentTypeAssociateWithHubSitesParameterSet
        .newBuilder()
        .withHubSiteUrls(hubSiteUrlsList)
        .withPropagateToExistingLists(propagateToExistingLists)
        .build())
    .buildRequest()
    .post();

```