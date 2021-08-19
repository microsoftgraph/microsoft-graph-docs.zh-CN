---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0eb2f259a1e351f57d644238b7fcc4b5257cf3f
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256941"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Admin.ServiceAnnouncement.Messages
    .Request()
    .GetAsync();

```