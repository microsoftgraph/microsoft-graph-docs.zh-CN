---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71073eb4716e644634bb269e32128b192d9ad4a31a651d8abe991f3304d61f14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103891"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["{call-id}"]
    .Mute(clientContext)
    .Request()
    .PostAsync();

```