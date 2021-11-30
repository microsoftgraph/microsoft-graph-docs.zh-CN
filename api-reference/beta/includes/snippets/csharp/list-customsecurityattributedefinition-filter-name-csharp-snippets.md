---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89b3b470460be3b2f7a910506697bc6839572dac
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224592"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customSecurityAttributeDefinitions = await graphClient.Directory.CustomSecurityAttributeDefinitions
    .Request()
    .Filter("name eq 'Project' and status eq 'Available'")
    .GetAsync();

```