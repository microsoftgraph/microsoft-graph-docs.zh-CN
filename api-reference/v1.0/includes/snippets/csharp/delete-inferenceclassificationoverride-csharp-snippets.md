---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 715948128a3f9a6b0ac16785a459219529ff8955
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.InferenceClassification.Overrides["98f5bdef-576a-404d-a2ea-07a3cf34af4r"]
    .Request()
    .DeleteAsync();

```