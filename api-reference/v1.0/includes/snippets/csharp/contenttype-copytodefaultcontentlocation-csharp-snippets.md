---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f7404c433eee15a92f0c044dbe937b5820e0622
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147630"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceFile = new ItemReference
{
    SharepointIds = new SharepointIds
    {
        ListId = "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0",
        ListItemId = "2"
    }
};

var destinationFileName = "newname.txt";

await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .CopyToDefaultContentLocation(sourceFile,destinationFileName)
    .Request()
    .PostAsync();

```