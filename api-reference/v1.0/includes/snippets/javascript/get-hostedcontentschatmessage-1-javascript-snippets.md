---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15ac7fa3abace4dada396244bb6f1376349893ed6739e70353f52ed6ebb59e22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let hostedContents = await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1615971548136/hostedContents')
    .get();

```