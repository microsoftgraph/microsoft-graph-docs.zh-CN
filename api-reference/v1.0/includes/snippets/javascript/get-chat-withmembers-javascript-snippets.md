---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9212c6ce53b3face74f63fafdb8cee54f9529bc2b82ce931ad6493a9643c52db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158720"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chat = await client.api('/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2')
    .expand('members')
    .get();

```