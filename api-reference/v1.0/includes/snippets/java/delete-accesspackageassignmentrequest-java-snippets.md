---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ebde64ca8cf623f0182b36bdd3a8967c3cfd916
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334563"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().assignmentRequests("{accessPackageAssignmentRequestId}")
    .buildRequest()
    .delete();

```