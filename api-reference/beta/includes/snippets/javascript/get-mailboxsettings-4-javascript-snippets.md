---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44723560b5a46a85f1bb2d70e25bfae90fefb143
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailboxSettings/userPurpose')
    .version('beta')
    .get();

```