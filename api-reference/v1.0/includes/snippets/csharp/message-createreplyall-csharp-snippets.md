---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e73b3879cbb0779addfce03e97b04fc9f723e7741e749000abb92528890d2a0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106722"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"]
    .CreateReplyAll(null,null)
    .Request()
    .PostAsync();

```