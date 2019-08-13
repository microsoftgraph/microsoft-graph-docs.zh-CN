---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 66ff4e8cac8f3adcb20deceb7bf323aee902f3a5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364945"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook
    .CloseSession()
    .Request()
    .Header("workbook-session-id","{session-id}")
    .PostAsync();

```