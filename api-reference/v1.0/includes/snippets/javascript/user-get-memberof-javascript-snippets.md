---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db259b541abe195f0183ea6c3563bc4b889ea46c1ce5411ddd165524d7a4546b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/users/{id}/memberOf')
    .get();

```