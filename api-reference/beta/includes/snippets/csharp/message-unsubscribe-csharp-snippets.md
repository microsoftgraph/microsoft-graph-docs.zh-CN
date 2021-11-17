---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddc3f9f859e5d9d957547bdb5481747b57e8ca6ad1f9ef471f49f6da68bfcf93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277604"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"]
    .Unsubscribe()
    .Request()
    .PostAsync();

```