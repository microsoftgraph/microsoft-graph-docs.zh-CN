---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e0993fccb32960c761e72391989af6cde70565c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038234"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"].Columns
    .Request()
    .GetAsync();

```