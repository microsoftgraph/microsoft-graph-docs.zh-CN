---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f6d3176469a4813d5e95a6a79c24db612c562cf
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528149"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TaskList baseTaskList = new TaskList();
baseTaskList.displayName = "Travel Plan";

graphClient.me().tasks().lists("AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFs")
    .buildRequest()
    .patch(baseTaskList);

```