---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83ec04cd8b980c9b390f9a10b0d4cd34af9a6c85
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217062"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffRequests = await graphClient.Teams["{teamId}"].Schedule.TimeOffRequests
    .Request()
    .GetAsync();

```