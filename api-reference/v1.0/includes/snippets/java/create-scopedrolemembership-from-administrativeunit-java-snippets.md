---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d581b38fef5fba4594a5180ae4d4c3670bcb578
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967388"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembership scopedRoleMembership = new ScopedRoleMembership();
scopedRoleMembership.roleId = "roleId-value";
Identity roleMemberInfo = new Identity();
roleMemberInfo.id = "id-value";
scopedRoleMembership.roleMemberInfo = roleMemberInfo;

graphClient.directory().administrativeUnits("{id}").scopedRoleMembers()
    .buildRequest()
    .post(scopedRoleMembership);

```