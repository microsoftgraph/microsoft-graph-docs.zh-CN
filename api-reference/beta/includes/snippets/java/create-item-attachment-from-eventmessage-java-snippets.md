---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31df94165c24b487ee82e208bad23f92cf5d076441eb63c8eb7db577f041200f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215851"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAttachment attachment = new ItemAttachment();
attachment.name = "name-value";
Message item = new Message();
attachment.item = item;

graphClient.me().events("{id}").attachments()
    .buildRequest()
    .post(attachment);

```