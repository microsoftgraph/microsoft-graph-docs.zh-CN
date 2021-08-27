---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ae4183fe48de8cf3679cfb7670725b110769169788cd6aadc110fe2fb652f01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902845"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages')
    .version('beta')
    .top(2)
    .get();

```