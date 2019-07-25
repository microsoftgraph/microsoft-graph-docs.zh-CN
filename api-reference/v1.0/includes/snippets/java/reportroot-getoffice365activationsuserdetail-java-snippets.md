---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6bce0a5f4c99ce45febdb650fa87010f62fac256
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881049"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365ActivationsUserDetail()
    .buildRequest()
    .get();

```