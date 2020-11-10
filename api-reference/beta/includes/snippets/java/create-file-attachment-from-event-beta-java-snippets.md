---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d621157f599d1bc58621637829df36ea1136ade
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954782"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAttachment attachment = new FileAttachment();
attachment.name = "menu.txt";
attachment.contentBytes = Base64.getDecoder().decode("bWFjIGFuZCBjaGVlc2UgdG9kYXk=");

graphClient.me().events("AAMkAGI1AAAt9AHjAAA=").attachments()
    .buildRequest()
    .post(attachment);

```