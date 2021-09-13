---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af1cb98c8bbf882ff07f072da82d11ff6cee8ecab73f515267b75e22768289e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107005"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{team-id}"].Schedule.OpenShiftChangeRequests["{openShiftChangeRequest-id}"]
    .Approve(message)
    .Request()
    .PostAsync();

```