---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9e74619b6c2c1ebae61f6ea26b22ec74a664dad95969fbcd0b114a55df88a36
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106033"
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