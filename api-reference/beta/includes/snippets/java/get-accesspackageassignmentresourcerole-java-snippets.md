---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36e747212698ce881d05304263180d9b18506e62
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976646"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentResourceRole accessPackageAssignmentResourceRole = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentResourceRoles("{id}")
    .buildRequest()
    .get();

```