---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d4a59f261353270988a6ed11346c5d4e0cc15d5b0e263b60275803ba805c35f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161378"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs
    .Request()
    .GetAsync();

```