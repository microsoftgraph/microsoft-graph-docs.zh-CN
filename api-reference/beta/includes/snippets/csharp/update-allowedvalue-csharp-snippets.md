---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e9b81cd793482afab0b47592e9357f697272d97
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223951"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedValue = new AllowedValue
{
    IsActive = false
};

await graphClient.Directory.CustomSecurityAttributeDefinitions["{customSecurityAttributeDefinition-id}"].AllowedValues["{allowedValue-id}"]
    .Request()
    .UpdateAsync(allowedValue);

```