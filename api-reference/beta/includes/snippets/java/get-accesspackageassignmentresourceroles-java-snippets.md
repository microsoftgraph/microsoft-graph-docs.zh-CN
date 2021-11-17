---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 954cc7786d362ff3c910aff33a2a704d833b3d319ad6242ab6bcf59ef826ec20
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902783"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentResourceRoleCollectionPage accessPackageAssignmentResourceRoles = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentResourceRoles()
    .buildRequest()
    .get();

```