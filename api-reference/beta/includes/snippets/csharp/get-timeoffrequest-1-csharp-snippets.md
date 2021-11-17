---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c99f03a21b0643b24d25175eead0176e5aea7110e23027c6698a36f81a3e8f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164065"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffRequest = await graphClient.Teams["{team-id}"].Schedule.TimeOffRequests["{timeOffRequest-id}"]
    .Request()
    .GetAsync();

```