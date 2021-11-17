---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c749873142ce92cb4ff6eff1fb9ca187d39204eab967225611cde3cb9d18f87e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218933"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{message-id}"].Mentions["{mention-id}"]
    .Request()
    .DeleteAsync();

```