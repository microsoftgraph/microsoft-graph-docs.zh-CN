---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9210b55f9400eeb44560f0732f273f560140101
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Admin.ServiceAnnouncement.Issues["{serviceHealthIssue-id}"]
    .IncidentReport()
    .Request()
    .GetAsync();

```