---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4bd8f5902993131822c1743f45a793fb63fb1caf9c21deec4eadbf96f38ad6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

await graphClient.Communications.Calls["{call-id}"].Participants["{participant-id}"]
    .Mute(clientContext)
    .Request()
    .PostAsync();

```