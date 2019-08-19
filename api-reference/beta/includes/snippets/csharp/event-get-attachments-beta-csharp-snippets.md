---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 783ded2727451ce3a79d1dcbbecdec8355d20d0a
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Me.Events["{id}"].Attachments
    .Request()
    .GetAsync();

```