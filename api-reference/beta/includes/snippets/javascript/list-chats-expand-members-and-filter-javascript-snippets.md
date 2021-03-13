---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 853697d3bb94e021f130b9f38a74f236d122403a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775743"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chats = await client.api('/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats')
    .version('beta')
    .filter('members/any(o: o/displayname eq \'Peter Parker\')')
    .expand('members')
    .get();

```