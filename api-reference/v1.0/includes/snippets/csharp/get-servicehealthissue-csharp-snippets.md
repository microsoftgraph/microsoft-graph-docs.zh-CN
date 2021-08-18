---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b0a97ec25ca9b30ef00b2a699647c00091a6ee9
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265928"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceHealthIssue = await graphClient.Admin.ServiceAnnouncement.Issues["{serviceHealthIssue-id}"]
    .Request()
    .GetAsync();

```