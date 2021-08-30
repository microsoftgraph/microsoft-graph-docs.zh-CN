---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a973aea4676b66cf2688a003f3bd490083444da8f77756da97c3f6b749ebb99
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Members["{conversationMember-id}"]
    .Request()
    .DeleteAsync();

```