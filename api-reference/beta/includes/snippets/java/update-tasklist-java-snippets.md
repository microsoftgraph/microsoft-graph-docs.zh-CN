---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 455643549b12926537e0828c12db131fe7840b22
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119983"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BaseTaskList baseTaskList = new BaseTaskList();
baseTaskList.displayName = "Travel Plan";

graphClient.me().tasks().lists("AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFs")
    .buildRequest()
    .patch(baseTaskList);

```