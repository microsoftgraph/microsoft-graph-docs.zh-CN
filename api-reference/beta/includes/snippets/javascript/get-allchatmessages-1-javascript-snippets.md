---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24ac64e5acf796b2bb64c3616f9694e0bfa0ab5d
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610731"
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