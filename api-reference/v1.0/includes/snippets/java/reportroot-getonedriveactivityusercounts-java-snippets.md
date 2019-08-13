---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0c9b9966b449ed6dd7583fe493f8c23e5b11337f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373975"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOneDriveActivityUserCounts("D7")
    .buildRequest()
    .get();

```