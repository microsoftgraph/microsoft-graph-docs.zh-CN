---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c98084d05731e73ba612030f60b4ac9eebb01d5af11731d9381172cbd33ecf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUsers = await graphClient.IdentityProtection.RiskyUsers
    .Request()
    .GetAsync();

```