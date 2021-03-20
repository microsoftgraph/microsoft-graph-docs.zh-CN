---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1be92f6a1b4dc91dba6cbeda18be74f9315f5b91
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974734"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicyCollectionPage accessPackageAssignmentPolicies = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies()
    .buildRequest()
    .get();

```