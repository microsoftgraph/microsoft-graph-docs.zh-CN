---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1b6e35f26f4e81051e96811a989042b6f3f48f1
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516238"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = await graphClient.IdentityGovernance.TermsOfUse.Agreements["{agreement-id}"]
    .Request()
    .Expand("files")
    .GetAsync();

```