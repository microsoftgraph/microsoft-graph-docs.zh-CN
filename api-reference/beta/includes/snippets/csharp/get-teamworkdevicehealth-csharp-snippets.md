---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bda3727be15764bc0f84707ac5f16f2a090be993
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349025"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkDeviceHealth = await graphClient.Teamwork.Devices["{teamworkDevice-id}"].Health
    .Request()
    .GetAsync();

```