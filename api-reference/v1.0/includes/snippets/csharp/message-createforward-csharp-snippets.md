---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a230bf451ae91801b85d940e0743230c2bb1efcc8802f8b886a0f1fc70dbb5eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"]
    .CreateForward(null,null,null)
    .Request()
    .PostAsync();

```