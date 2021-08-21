---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3012459558e7e0e06ce83e01f1aeb78cccb87192c299497efaa5b219a7c16d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273952"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignments = await graphClient.PrivilegedRoleAssignments
    .Request()
    .Filter("isElevated eq true and expirationDateTime ne null or isElevated eq false")
    .GetAsync();

```