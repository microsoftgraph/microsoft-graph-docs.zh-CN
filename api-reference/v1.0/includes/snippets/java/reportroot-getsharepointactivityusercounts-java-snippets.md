---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 351b236ba470b5bcd60bbc732da7cdbd40564d32
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893526"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointActivityUserCounts('D7')
    .buildRequest()
    .get();

```