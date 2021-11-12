---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 830741469385fcf0bf230def526736619c36c72f04a957a03f03c9438a52e773
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902555"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembership scopedRoleMembership = new ScopedRoleMembership();
scopedRoleMembership.roleId = "roleId-value";
Identity roleMemberInfo = new Identity();
roleMemberInfo.id = "id-value";
scopedRoleMembership.roleMemberInfo = roleMemberInfo;

graphClient.administrativeUnits("{id}").scopedRoleMembers()
    .buildRequest()
    .post(scopedRoleMembership);

```