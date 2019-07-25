---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5447e3f62fa1b43600316004c35aafc6bbc1139a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872414"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessActivityUserCountsCollectionPage getSkypeForBusinessActivityUserCounts = graphClient.reports()
    .getSkypeForBusinessActivityUserCounts('D7')
    .buildRequest()
    .get();

```