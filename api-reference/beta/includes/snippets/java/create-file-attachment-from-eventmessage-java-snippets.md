---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec42f5ae840deca740226c7ee7c947ccee026996
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983185"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAttachment attachment = new FileAttachment();
attachment.name = "name-value";
attachment.contentType = "contentType-value";
attachment.isInline = false;
attachment.contentLocation = "contentLocation-value";
attachment.contentBytes = Base64.getDecoder().decode("contentBytes-value");

graphClient.me().messages("{id}").attachments()
    .buildRequest()
    .post(attachment);

```