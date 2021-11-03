---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fbfe36c51cdf3c3f0246fb22b0506c2e686dee7
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePlans = await graphClient.DeviceManagement.VirtualEndpoint.ServicePlans
    .Request()
    .GetAsync();

```