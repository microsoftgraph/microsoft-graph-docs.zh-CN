---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d7139993fd6bb48e98cfda07a6de9a6eb92656e9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886648"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getTeamsUserActivityUserCounts('D7')
    .buildRequest()
    .get();

```