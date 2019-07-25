---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eb3e5fd8aa5f0be59065a5a5bc5785048b0dbdc5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871579"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsUserActivityUserDetailCollectionPage getTeamsUserActivityUserDetail = graphClient.reports()
    .getTeamsUserActivityUserDetail('D7')
    .buildRequest()
    .get();

```