---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba268a6f62e55e9fbdbec9250e0d0aee4026e11343e2fe7261795a6ff36c069d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158685"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{team-id}"].Schedule.TimeOffRequests["{timeOffRequest-id}"]
    .Approve(message)
    .Request()
    .PostAsync();

```