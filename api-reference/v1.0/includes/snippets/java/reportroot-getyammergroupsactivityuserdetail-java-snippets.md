---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6b310a6c32c74401fa72d081a6971fbe50b2ba0f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320210"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerGroupsActivityDetail("D7")
    .buildRequest()
    .get();

```