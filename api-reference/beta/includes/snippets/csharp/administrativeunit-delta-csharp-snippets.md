---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb307960cbd4ae5727bfd222625c25b0a57b0aa5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.AdministrativeUnits
    .Delta()
    .Request()
    .GetAsync();

```