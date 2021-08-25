---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 439f810f37fc90b21b040e56d7c6056c52a9ec3e1112b2b5f7e169d508170acf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hubSiteUrls = new List<String>()
{
    "https://graph.microsoft.com/beta/sites/id"
};

var propagateToExistingLists = false;

await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .AssociateWithHubSites(hubSiteUrls,propagateToExistingLists)
    .Request()
    .PostAsync();

```