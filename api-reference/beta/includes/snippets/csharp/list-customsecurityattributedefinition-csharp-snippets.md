---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bbe4f99a589c25c2a9ca680ca789c3cd279c0a5
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224584"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customSecurityAttributeDefinitions = await graphClient.Directory.CustomSecurityAttributeDefinitions
    .Request()
    .GetAsync();

```