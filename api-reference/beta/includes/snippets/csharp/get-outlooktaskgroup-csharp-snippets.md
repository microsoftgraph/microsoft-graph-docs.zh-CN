---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cec59bf212ecec7f9fe087354b0e30acd26379ab23bac71b3a73b88453403364
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903674"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskGroup = await graphClient.Me.Outlook.TaskGroups["{outlookTaskGroup-id}"]
    .Request()
    .GetAsync();

```