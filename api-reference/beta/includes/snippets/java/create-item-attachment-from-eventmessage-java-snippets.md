---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02b1e7c4ce0a4bc0eb4edb397caf8bc1533301b9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965733"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAttachment attachment = new ItemAttachment();
attachment.name = "name-value";
attachment.item = "message or event entity";

graphClient.me().events("{id}").attachments()
    .buildRequest()
    .post(attachment);

```