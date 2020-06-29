---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f92ac31be2eb3ef287fab64544f4885b2d7d06e3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44900270"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "I will probably be able to make it.";

var sendResponse = true;

await graphClient.Me.Events["AAMkADADVj3fyAABZ5ieyAAA="]
    .TentativelyAccept(comment,sendResponse)
    .Request()
    .PostAsync();

```