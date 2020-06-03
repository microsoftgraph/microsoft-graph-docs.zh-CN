---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83ec04cd8b980c9b390f9a10b0d4cd34af9a6c85
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44215806"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffRequests = await graphClient.Teams["{teamId}"].Schedule.TimeOffRequests
    .Request()
    .GetAsync();

```