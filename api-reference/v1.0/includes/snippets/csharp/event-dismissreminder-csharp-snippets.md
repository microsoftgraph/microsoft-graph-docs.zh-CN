---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f48f47eae762be230e5087348dd3427d9773f490e92324648522394f66b96794
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{event-id}"]
    .DismissReminder()
    .Request()
    .PostAsync();

```