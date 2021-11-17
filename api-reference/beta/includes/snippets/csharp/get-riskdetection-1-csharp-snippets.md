---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fd5dd6366093215b2eb4d5a9d7712a4e262eef6c899ead0657730b60f92ea36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218446"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetections = await graphClient.RiskDetections
    .Request()
    .GetAsync();

```