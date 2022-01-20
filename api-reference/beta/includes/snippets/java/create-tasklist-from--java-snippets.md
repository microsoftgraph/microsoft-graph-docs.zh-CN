---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 924d1b2eb1e009fb958600ba8c55719e2bfa25a7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098559"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BaseTaskList baseTaskList = new BaseTaskList();
baseTaskList.displayName = "Shopping list";

graphClient.me().tasks().lists()
    .buildRequest()
    .post(baseTaskList);

```