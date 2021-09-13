---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ac94fff7b68cea19147a8d2d42d438fa60a014a65bd52e8a7caa8c00850e39f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334001"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "fd1c7836-4d84-4e24-b6aa-23188688cc54";

await graphClient.Communications.Calls["{call-id}"]
    .SubscribeToTone(clientContext)
    .Request()
    .PostAsync();

```