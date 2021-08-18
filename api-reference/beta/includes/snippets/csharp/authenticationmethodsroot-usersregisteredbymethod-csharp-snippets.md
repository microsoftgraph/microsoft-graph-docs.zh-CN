---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf1d685182e17a24de38e63d264b23547ffd32e57f03d8edda5446503f993366
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105057"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userRegistrationMethodSummary = await graphClient.Reports.AuthenticationMethods
    .UsersRegisteredByMethod(IncludedUserTypes.All,IncludedUserRoles.All)
    .Request()
    .GetAsync();

```