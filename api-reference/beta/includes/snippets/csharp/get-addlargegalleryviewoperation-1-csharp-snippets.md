---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27168f481bf227217fb46d8d246c75e29f5755f4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204153"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var commsOperation = await graphClient.Communications.Calls["{call-id}"].Operations["{commsOperation-id}"]
    .Request()
    .GetAsync();

```