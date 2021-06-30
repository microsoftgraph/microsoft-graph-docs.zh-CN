---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9210b55f9400eeb44560f0732f273f560140101
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Admin.ServiceAnnouncement.Issues["{serviceHealthIssue-id}"]
    .IncidentReport()
    .Request()
    .GetAsync();

```