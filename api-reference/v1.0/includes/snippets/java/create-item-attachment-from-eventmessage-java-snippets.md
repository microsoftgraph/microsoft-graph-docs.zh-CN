---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea45986918df0f1f662e38de00531e141179453b
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910541"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAttachment attachment = new ItemAttachment();
attachment.name = "name-value";
Message item = new Message();
attachment.item = item;

graphClient.me().events("{id}").attachments()
    .buildRequest()
    .post(attachment);

```