---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e9dc0d103a417eddaa975f980568ff07fb37323
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618355"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTask = await graphClient.Planner.Tasks["01gzSlKkIUSUl6DF_EilrmQAKDhh"]
    .Request()
    .GetAsync();

```