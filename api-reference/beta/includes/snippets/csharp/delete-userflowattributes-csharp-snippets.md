---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d62a28bd60753fe3c538ea8ac8f328ba18104290651285c09e897b3f3bf81a49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161430"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.UserFlowAttributes["{identityUserFlowAttribute-id}"]
    .Request()
    .DeleteAsync();

```