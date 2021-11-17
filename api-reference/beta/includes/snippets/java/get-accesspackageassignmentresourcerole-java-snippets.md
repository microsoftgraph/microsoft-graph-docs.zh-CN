---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66a743d2577ebfb24de677813e32b9609a4f6ab52b9711f3e365a7efeac2ab10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158649"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentResourceRole accessPackageAssignmentResourceRole = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentResourceRoles("{id}")
    .buildRequest()
    .get();

```