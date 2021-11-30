---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05e40172aa9c2c27526c4aef98aeab2bdfd450f3
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225640"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customSecurityAttributeDefinition = new CustomSecurityAttributeDefinition
{
    Status = "Deprecated"
};

await graphClient.Directory.CustomSecurityAttributeDefinitions["{customSecurityAttributeDefinition-id}"]
    .Request()
    .UpdateAsync(customSecurityAttributeDefinition);

```