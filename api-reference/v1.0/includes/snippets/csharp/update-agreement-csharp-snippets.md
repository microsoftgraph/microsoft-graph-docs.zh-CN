---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b9a0a3059026c7097cf1ef00a53819aebd19a5f2aee63de0f995f86097a9502
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219398"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = new Agreement
{
    DisplayName = "Sample ToU display name",
    IsViewingBeforeAcceptanceRequired = true
};

await graphClient.IdentityGovernance.TermsOfUse.Agreements["{agreement-id}"]
    .Request()
    .UpdateAsync(agreement);

```