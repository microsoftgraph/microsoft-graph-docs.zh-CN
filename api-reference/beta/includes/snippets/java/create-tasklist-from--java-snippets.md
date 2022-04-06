---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a4a559b62bc13942655cf5ff5f50be9da60bd31
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528147"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TaskList baseTaskList = new TaskList();
baseTaskList.displayName = "Shopping list";

graphClient.me().tasks().lists()
    .buildRequest()
    .post(baseTaskList);

```