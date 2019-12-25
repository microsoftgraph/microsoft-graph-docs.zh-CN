---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f810d2466b0cdff9d594384c10444d18db1698d5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["57dab8b1-894c-409a-b240-bd8beae78896"]
    .Unmute(clientContext)
    .Request()
    .PostAsync();

```