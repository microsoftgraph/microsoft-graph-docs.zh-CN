---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ca0fede39471ed355ac5275df731e0d01fc750a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentSharingSessions = await graphClient.Communications.Calls["{call-id}"].ContentSharingSessions
    .Request()
    .GetAsync();

```