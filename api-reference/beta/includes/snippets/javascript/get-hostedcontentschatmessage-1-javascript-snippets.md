---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73315e09c94c4a8f072d52911e8b9bc1e90c3f9300989af0a8c4af584538721f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218519"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let hostedContents = await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents')
    .version('beta')
    .get();

```