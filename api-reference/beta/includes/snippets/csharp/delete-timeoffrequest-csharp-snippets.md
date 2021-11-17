---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adeb87ffea85538595cf7566d15351b746bb9b031704e078b16c048ce3ca3e44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105505"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.TimeOffRequests["{timeOffRequest-id}"]
    .Request()
    .DeleteAsync();

```