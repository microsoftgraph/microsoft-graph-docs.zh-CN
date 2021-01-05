---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91d87a2c07d060f20172d33a4bf50b31385cc1b9
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752894"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats')
    .version('beta')
    .filter('members/any(o: o/displayname eq 'Peter Parker')')
    .expand('members')
    .get();

```