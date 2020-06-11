---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3aa1a6e680c317d55d0137e7dece9b9c45a76299
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685218"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAttachment attachment = new ItemAttachment();
attachment.name = "name-value";
attachment.item = "{message or event entity}";

graphClient.me().events("{id}").attachments()
    .buildRequest()
    .post(attachment);

```