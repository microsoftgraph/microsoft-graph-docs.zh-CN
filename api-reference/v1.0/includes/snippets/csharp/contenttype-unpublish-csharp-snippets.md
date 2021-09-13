---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d169986ff933d2f948fe9df54a9fab5d7e4d3ff1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038107"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .Unpublish()
    .Request()
    .PostAsync();

```