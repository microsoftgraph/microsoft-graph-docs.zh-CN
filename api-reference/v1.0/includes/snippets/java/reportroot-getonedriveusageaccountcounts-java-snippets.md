---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 926df651377f5c6fc5ae04b7d49a13cb64b93847
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327597"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveUsageAccountCounts("D7")
    .buildRequest()
    .get();

```