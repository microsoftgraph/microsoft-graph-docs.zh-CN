---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1992cd1afda1b18ae9a33e40c4e68e28ee8e595f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874030"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailActivitySummaryCollectionPage getEmailActivityUserCounts = graphClient.reports()
    .getEmailActivityUserCounts('D7')
    .buildRequest()
    .get();

```