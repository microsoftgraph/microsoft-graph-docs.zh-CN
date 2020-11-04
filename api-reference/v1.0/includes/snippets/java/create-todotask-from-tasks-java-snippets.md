---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2af6661ebeedbf1a07de302aea6ab56ebb4aa2c
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904431"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTask todoTask = new TodoTask();
todoTask.title = "A new task";
LinkedList<LinkedResource> linkedResourcesList = new LinkedList<LinkedResource>();
LinkedResource linkedResources = new LinkedResource();
linkedResources.webUrl = "http://microsoft.com";
linkedResources.applicationName = "Microsoft";
linkedResources.displayName = "Microsoft";
linkedResourcesList.add(linkedResources);
todoTask.linkedResources = linkedResourcesList;

graphClient.me().todo().lists("AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM").tasks()
    .buildRequest()
    .post(todoTask);

```