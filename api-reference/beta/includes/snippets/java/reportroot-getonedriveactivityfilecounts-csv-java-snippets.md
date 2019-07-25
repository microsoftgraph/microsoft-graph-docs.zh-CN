---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 07d138de057f8a88753fdf4d51c38a6615e08b7d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873149"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteActivitySummaryCollectionPage getOneDriveActivityFileCounts = graphClient.reports()
    .getOneDriveActivityFileCounts('D7')
    .buildRequest()
    .get();

```