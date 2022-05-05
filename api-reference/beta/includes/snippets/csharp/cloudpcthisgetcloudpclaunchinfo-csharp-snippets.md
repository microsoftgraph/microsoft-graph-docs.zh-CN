---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 601d077cddf0420d1e46fda1a15851e13e58eb90
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcLaunchInfo = await graphClient.Me.CloudPCs["{cloudPC-id}"]
    .GetCloudPcLaunchInfo()
    .Request()
    .GetAsync();

```