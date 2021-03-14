---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f924b5a13b55277516313b17bf0501771ec9eb6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785124"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Members["{conversationMember-id}"]
    .Request()
    .DeleteAsync();

```