---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b2d8147a41dd273e9815c7ad9250db9b40fc84e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100542"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages')
    .version('beta')
    .orderby('createdDateTime')
    .top(2)
    .get();

```