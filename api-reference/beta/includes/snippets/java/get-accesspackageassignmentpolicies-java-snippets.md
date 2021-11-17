---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d58edd9dbbc866471314b8ebf9db09aa93e7c825f91c777305fe84d6a76512f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902812"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicyCollectionPage accessPackageAssignmentPolicies = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies()
    .buildRequest()
    .get();

```