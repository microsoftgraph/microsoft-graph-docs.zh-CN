---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afde9f85b9edb37e2f891dc8fa6eecc7b93d05a11203078bd20387b42fc9e249
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221498"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me
    .InvalidateAllRefreshTokens()
    .Request()
    .PostAsync();

```