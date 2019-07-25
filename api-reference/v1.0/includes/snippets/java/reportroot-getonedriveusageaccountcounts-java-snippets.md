---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2ef27788f3b07a80a79c446943c74855f8d505c6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893707"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveUsageAccountCounts('D7')
    .buildRequest()
    .get();

```