---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66aebf26996484fd4d3014a3df45fc74239b92c3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201682"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var windowsHelloForBusinessMethods = await graphClient.Users["{user-id}"].Authentication.WindowsHelloForBusinessMethods
    .Request()
    .GetAsync();

```