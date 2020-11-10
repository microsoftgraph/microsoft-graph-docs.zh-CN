---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6c4ce188d74dd8b413ad63db684d4d3ee42d81a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952118"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequest accessPackageAssignmentRequest = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests("{id}")
    .buildRequest()
    .get();

```