---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0b29ba7c010a92aea1c29016ef90f93b590f8f9e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893488"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointSiteUsageDetail('D7')
    .buildRequest()
    .get();

```