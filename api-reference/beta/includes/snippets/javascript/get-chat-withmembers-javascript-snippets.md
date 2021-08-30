---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6e9811a024794fef8db4fba91474f9581a232d865b397d8c19d1674ace229e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chat = await client.api('/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2')
    .version('beta')
    .expand('members')
    .get();

```