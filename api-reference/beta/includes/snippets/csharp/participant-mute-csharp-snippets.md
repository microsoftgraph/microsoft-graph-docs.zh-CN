---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62b891e80df7c2a6f2b1934bcf0ca9216b43c42c
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

await graphClient.Communications.Calls["57dab8b1-894c-409a-b240-bd8beae78896"].Participants["2765eb15-01f8-47c6-b12b-c32111a4a86f"]
    .Mute(clientContext)
    .Request()
    .PostAsync();

```