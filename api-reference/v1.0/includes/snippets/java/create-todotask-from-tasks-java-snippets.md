---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73f4711ade99495391369dcf1c75d7dddc50f09439f22b689bab75d5f15f5dff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTask todoTask = new TodoTask();
todoTask.title = "A new task";
LinkedList<LinkedResource> linkedResourcesList = new LinkedList<LinkedResource>();
LinkedResource linkedResources = new LinkedResource();
linkedResources.webUrl = "http://microsoft.com";
linkedResources.applicationName = "Microsoft";
linkedResources.displayName = "Microsoft";
linkedResourcesList.add(linkedResources);
LinkedResourceCollectionResponse linkedResourceCollectionResponse = new LinkedResourceCollectionResponse();
linkedResourceCollectionResponse.value = linkedResourcesList;
LinkedResourceCollectionPage linkedResourceCollectionPage = new LinkedResourceCollectionPage(linkedResourceCollectionResponse, null);
todoTask.linkedResources = linkedResourceCollectionPage;

graphClient.me().todo().lists("AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM").tasks()
    .buildRequest()
    .post(todoTask);

```