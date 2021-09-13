---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cbde1bb2342edda0dd5ba854d5e31f61b7ad815c838502df255cd95e0e50b13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105305"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTask todoTask = new TodoTask();
DateTimeTimeZone dueDateTime = new DateTimeTimeZone();
dueDateTime.dateTime = "2020-07-25T16:00:00";
dueDateTime.timeZone = "Eastern Standard Time";
todoTask.dueDateTime = dueDateTime;

graphClient.me().todo().lists("AAMkADA1MTHgwAAA=").tasks("721a35e2-35e2-721a-e235-1a72e2351a72")
    .buildRequest()
    .patch(todoTask);

```