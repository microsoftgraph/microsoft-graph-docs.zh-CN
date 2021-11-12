---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f4e0bc13f4b05c631d541de561961ac607f2cb4b6b26af2e0de981a8cf1c3e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103879"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAttachment attachment = new FileAttachment();
attachment.name = "menu.txt";
attachment.contentBytes = Base64.getDecoder().decode("bWFjIGFuZCBjaGVlc2UgdG9kYXk=");

graphClient.me().events("AAMkAGI1AAAt9AHjAAA=").attachments()
    .buildRequest()
    .post(attachment);

```