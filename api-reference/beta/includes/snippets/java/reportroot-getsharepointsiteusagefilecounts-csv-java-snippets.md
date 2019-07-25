---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2e8994350132067edd686f44af1254b371c37596
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872643"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointSiteUsageFileCountsCollectionPage getSharePointSiteUsageFileCounts = graphClient.reports()
    .getSharePointSiteUsageFileCounts('D7')
    .buildRequest()
    .get();

```