---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57ddc40bd444c791a6c1d3f2d21a6820871c07bee7e42d23c9cafabb355d36e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220916"
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