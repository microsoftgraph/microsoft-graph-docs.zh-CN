---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6c43d8affe7376da0b52117331f1aa43c858e5c
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethod = await graphClient.Me.Authentication.Methods["{id}"]
    .Request()
    .GetAsync();

```