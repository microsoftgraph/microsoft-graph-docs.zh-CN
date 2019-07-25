---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4b0dc4cc0c2aeaa733c0b5f7f0429527261ace0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884945"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Me.MemberOf
    .Request()
    .GetAsync();

```