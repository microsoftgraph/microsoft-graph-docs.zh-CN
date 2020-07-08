---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bec088e1346fb1f9a300c8a57b1497aa61f799a
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Education.Users
    .Delta()
    .Request()
    .GetAsync();

```