---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3537798c5b9ee9afbaa85747bbd7315abbb0d3e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Communications.Calls["{call-id}"]
    .KeepAlive()
    .Request()
    .PostAsync();

```