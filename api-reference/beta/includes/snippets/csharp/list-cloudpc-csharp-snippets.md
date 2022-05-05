---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d6bdec1977ab194645d1a3eb61473d5d71bb6ae
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211982"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPCs = await graphClient.Me.CloudPCs
    .Request()
    .GetAsync();

```