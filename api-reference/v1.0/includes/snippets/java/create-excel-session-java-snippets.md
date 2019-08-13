---
description: 自动生成的文件。 不修改
ms.openlocfilehash: be431cf334064cbba704d566a2335f74c24b237a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365546"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean persistChanges = True;

graphClient.me().drive().items("{id}").workbook()
    .createSession(persistChanges)
    .buildRequest()
    .post();

```