---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 66efae40393531d0920a28eb3359c78e51bb860f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373716"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityFileCounts("D7")
    .buildRequest()
    .get();

```