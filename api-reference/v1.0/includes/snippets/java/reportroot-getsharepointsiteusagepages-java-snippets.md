---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c502a39789fc6af25e0ff9bf7960a56ec71fef26
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893404"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointSiteUsagePages('D7')
    .buildRequest()
    .get();

```