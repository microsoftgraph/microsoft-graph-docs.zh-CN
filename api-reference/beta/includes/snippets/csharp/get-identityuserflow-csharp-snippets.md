---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab625cda64991eecfdec0de8a131a9dfe5682467cb4d2f2d0949995f281a3821
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328780"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlow = await graphClient.Identity.UserFlows["{identityUserFlow-id}"]
    .Request()
    .GetAsync();

```