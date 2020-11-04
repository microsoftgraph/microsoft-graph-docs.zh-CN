---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0f083307a9f71afb8212badb06168243574bf68
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904397"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTaskList todoTaskList = new TodoTaskList();
todoTaskList.displayName = "Vacation Plan";

graphClient.me().todo().lists("AAMkADIyAAAhrbPWAAA=")
    .buildRequest()
    .patch(todoTaskList);

```