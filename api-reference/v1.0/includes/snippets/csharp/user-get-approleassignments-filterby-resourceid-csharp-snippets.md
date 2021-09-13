---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5619fce7c2a812451bf8d323f2f1349cf791e36b9d590ae7776fe7baefb1203c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106756"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.Users["{user-id}"].AppRoleAssignments
    .Request()
    .Filter("resourceId eq 8e881353-1735-45af-af21-ee1344582a4d")
    .GetAsync();

```