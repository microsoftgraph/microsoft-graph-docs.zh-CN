---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cb3b79bb651460c085316468a00acd6434ffa7009ea50b6004683eb3fd587d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.Tasks["{outlookTask-id}"]
    .Complete()
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .PostAsync();

```