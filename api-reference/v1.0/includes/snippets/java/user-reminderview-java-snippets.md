---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5bc86455847b86622cc2c2eb310b080cb9f600a0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372575"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IReminderCollectionPage reminderView = graphClient.me()
    .reminderView("2017-06-05T10:00:00.0000000","2017-06-11T11:00:00.0000000")
    .buildRequest()
    .get();

```