---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6caf8484e523a4d746c8b15290e848c6fef56561
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373694"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityGroupCounts("D7")
    .buildRequest()
    .get();

```