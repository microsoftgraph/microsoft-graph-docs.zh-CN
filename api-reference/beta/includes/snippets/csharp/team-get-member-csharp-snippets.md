---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19b92dedde3888dac42e1e2238ed30c892f63b83a276abd8adcda75b294f6371
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903731"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = await graphClient.Teams["{team-id}"].Members["{conversationMember-id}"]
    .Request()
    .GetAsync();

```