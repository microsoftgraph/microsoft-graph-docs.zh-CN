---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fe249f0d47c358ce996356075b068e1dd80b4f79
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893710"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveActivityFileCounts('D7')
    .buildRequest()
    .get();

```