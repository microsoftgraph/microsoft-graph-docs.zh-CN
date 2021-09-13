---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec262b9291f9d9b0931b254cc3835714e5a8e5cd9384eff111d8365d894b2a1f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903329"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    IsRead = true
};

await graphClient.Me.Messages["{message-id}"]
    .Request()
    .UpdateAsync(message);

```