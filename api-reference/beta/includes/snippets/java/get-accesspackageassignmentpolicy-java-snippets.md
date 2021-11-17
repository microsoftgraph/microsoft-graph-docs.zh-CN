---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9438fb52d607c9f508df5265bebd32cbe75b56a8733bb370ba203e7435b4e1e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902816"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicy accessPackageAssignmentPolicy = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies("{id}")
    .buildRequest()
    .get();

```