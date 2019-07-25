---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eb1fc3148fdfe95128bc4e225424db81ccc612f0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875232"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IProvisioningObjectSummaryCollectionPage directoryProvisioning = graphClient.auditLogs().directoryProvisioning()
    .buildRequest()
    .get();

```