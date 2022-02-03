---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e16d2c12d710c967a28703b4cee9c335a6baa6c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343824"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkDeviceConfiguration = await graphClient.Teamwork.Devices["{teamworkDevice-id}"].Configuration
    .Request()
    .GetAsync();

```