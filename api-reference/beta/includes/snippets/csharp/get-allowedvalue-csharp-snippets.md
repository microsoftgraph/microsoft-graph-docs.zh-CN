---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4d9656c5905cb86dc64bd774999e988b7eec893
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedValue = await graphClient.Directory.CustomSecurityAttributeDefinitions["{customSecurityAttributeDefinition-id}"].AllowedValues["{allowedValue-id}"]
    .Request()
    .GetAsync();

```