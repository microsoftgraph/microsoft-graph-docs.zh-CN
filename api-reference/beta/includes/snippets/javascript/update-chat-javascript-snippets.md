---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 501d2f5592d2b7d5876116ca876be23bd7fdeced610a7c08b1d8974283250fda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162509"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chat = {
    topic: 'Group chat title update'
};

await client.api('/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2')
    .version('beta')
    .update(chat);

```