---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2bdc5dd3a6111e0f54b5b266ffec0c38229d56a4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874066"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailActivitySummaryCollectionPage getEmailActivityCounts = graphClient.reports()
    .getEmailActivityCounts('D7')
    .buildRequest()
    .get();

```