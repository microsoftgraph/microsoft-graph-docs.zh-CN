---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 527959e4261f56a58f0ae015facaf684c90faf963cd77feac627c5e4218b3341
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902797"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequest accessPackageAssignmentRequest = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests("{id}")
    .buildRequest()
    .get();

```