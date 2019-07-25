---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1f609a2894300550a6b22d787cda075b47660cc2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893789"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365ServicesUserCounts('D7')
    .buildRequest()
    .get();

```