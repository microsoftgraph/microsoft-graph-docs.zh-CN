---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91de68993541d940b8aa0e34f398c3a20a472e73733f3bda447ea12d2b62408f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904032"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAttachment attachment = new FileAttachment();
attachment.name = "smile";
attachment.contentBytes = Base64.getDecoder().decode("a0b1c76de9f7=");

graphClient.me().messages("AAMkpsDRVK").attachments()
    .buildRequest()
    .post(attachment);

```