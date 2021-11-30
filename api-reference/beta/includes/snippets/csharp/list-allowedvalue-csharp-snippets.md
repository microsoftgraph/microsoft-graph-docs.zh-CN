---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b001b9c7b63d4843b7120c3176c48636967f0622
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedValues = await graphClient.Directory.CustomSecurityAttributeDefinitions["{customSecurityAttributeDefinition-id}"].AllowedValues
    .Request()
    .GetAsync();

```