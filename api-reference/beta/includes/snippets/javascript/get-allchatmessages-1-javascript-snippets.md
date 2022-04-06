---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e9cf299518a7d1427e8f4acbb713815ae6553cd
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages')
    .version('beta')
    .orderby('createdDateTime desc')
    .top(2)
    .get();

```