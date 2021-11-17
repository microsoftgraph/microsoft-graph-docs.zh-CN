---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b53cff69aba1bed89f73bf91616cf4ec1a58f2c1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "61021911"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mobilityManagementPolicy = await graphClient.Policies.MobileDeviceManagementPolicies["{mobilityManagementPolicy-id}"]
    .Request()
    .GetAsync();

```