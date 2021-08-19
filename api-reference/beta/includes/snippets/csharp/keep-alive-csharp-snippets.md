---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e12e08b3f432be4a0eec716ba93affaeaf2efd97fa0040005212781131358c78
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161594"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["{call-id}"]
    .KeepAlive()
    .Request()
    .PostAsync();

```