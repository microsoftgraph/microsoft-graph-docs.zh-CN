---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00cfbf2ff6d0239d46bb65e98c78463331d6b0b3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771132"
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