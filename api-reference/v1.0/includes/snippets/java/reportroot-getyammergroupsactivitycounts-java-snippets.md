---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3c9e12b4d39aa8051ad44be57879b4826d2826d6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320209"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerGroupsActivityCounts("D7")
    .buildRequest()
    .get();

```