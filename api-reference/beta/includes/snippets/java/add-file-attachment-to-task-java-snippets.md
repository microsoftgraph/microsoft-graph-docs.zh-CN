---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63d6d366b9b225c9a7d846fe8e31498c363bebb5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974054"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAttachment attachment = new FileAttachment();
attachment.name = "menu.txt";
attachment.contentBytes = Base64.getDecoder().decode("bWFjIGFuZCBjaGVlc2UgdG9kYXk=");

graphClient.me().outlook().tasks("AAMkADAAAANXbdnAAA=").attachments()
    .buildRequest()
    .post(attachment);

```