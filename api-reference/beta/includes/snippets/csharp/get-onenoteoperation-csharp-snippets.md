---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e9f26bff8ea24aae51757eaacfe568fdd368fe6712a4fee1442d7a3a37d1a93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219742"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteOperation = await graphClient.Me.Onenote.Operations["{onenoteOperation-id}"]
    .Request()
    .GetAsync();

```