---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6644adef96f05953c3b539f38fe294bfe4d9cea1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983555"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAttachment attachment = new FileAttachment();
attachment.name = "smile";
attachment.contentBytes = Base64.getDecoder().decode("R0lGODdhEAYEAA7");

graphClient.me().messages("AAMkpsDRVK").attachments()
    .buildRequest()
    .post(attachment);

```