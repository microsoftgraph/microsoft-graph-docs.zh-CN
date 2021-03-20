---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7348e8ef16a4b258f4241e8e804d341c5af79e99
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953891"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffRequests = await graphClient.Teams["{team-id}"].Schedule.TimeOffRequests
    .Request()
    .GetAsync();

```