---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ebf3d761c620f73773efaff47edcd5be0f1dbd27
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894378"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getMailboxUsageMailboxCounts('D7')
    .buildRequest()
    .get();

```