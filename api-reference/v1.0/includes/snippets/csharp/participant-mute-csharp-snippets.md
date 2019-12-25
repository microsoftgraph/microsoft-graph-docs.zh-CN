---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62b891e80df7c2a6f2b1934bcf0ca9216b43c42c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865802"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

await graphClient.Communications.Calls["57dab8b1-894c-409a-b240-bd8beae78896"].Participants["2765eb15-01f8-47c6-b12b-c32111a4a86f"]
    .Mute(clientContext)
    .Request()
    .PostAsync();

```