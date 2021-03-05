---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d02d2a1da160a784327d00ac06cce4f37e14ed7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465418"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats')
    .version('beta')
    .filter('members/any(o: o/displayname eq \'Peter Parker\')')
    .expand('members')
    .get();

```