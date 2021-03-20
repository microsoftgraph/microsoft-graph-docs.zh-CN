---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a01961b19f3035bcfa94dbad1d4af5cc1534fb14
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978809"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userRegistrationFeatureSummary = await graphClient.Reports.AuthenticationMethods
    .UsersRegisteredByFeature(IncludedUserTypes.All,IncludedUserRoles.All)
    .Request()
    .GetAsync();

```