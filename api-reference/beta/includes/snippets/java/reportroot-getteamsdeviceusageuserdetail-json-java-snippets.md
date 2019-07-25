---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b8029ad276949f1d138d9aef2a23d22763565283
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871764"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsDeviceUsageUserDetailCollectionPage getTeamsDeviceUsageUserDetail = graphClient.reports()
    .getTeamsDeviceUsageUserDetail('D7')
    .buildRequest()
    .get();

```