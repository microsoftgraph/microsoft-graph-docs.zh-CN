---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1e0a69fb831690d1605f5d0d23510bd9f7ecf4fe
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893664"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveUsageAccountDetail('D7')
    .buildRequest()
    .get();

```