---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 324cf49890987c135d028c5d13f51bc5f537ee9c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policies = await graphClient.ConditionalAccess.Policies
    .Request()
    .Filter("displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'")
    .GetAsync();

```