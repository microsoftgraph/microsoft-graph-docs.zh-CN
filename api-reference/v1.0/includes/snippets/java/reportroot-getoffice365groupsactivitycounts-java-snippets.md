---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5840f68537fd54145ad19f9efdf97529d41c73bb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893972"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityCounts('D7')
    .buildRequest()
    .get();

```