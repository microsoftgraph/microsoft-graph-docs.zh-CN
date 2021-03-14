---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 368556be1423f47ca2ff68c6a82b4151d52abd02
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802207"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = await graphClient.Devices["{device-id}"]
    .Request()
    .GetAsync();

```