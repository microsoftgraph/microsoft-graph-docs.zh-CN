---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a192d2f661abf51533c5a66f706d41a679a07fc9
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544210"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAttachment attachment = new FileAttachment();
attachment.name = "name-value";
attachment.contentType = "contentType-value";
attachment.isInline = false;
attachment.contentLocation = "contentLocation-value";
attachment.contentBytes = "base64-contentBytes-value";

graphClient.me().messages("{id}").attachments()
    .buildRequest()
    .post(attachment);

```