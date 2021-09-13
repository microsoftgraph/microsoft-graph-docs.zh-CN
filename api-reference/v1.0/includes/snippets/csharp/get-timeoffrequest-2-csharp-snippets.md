---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29a0024cf153877b555fadfa5435bfd0b9c53d80ca9bac3f794f6e1e71139e84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409318"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffRequests = await graphClient.Teams["{team-id}"].Schedule.TimeOffRequests
    .Request()
    .GetAsync();

```