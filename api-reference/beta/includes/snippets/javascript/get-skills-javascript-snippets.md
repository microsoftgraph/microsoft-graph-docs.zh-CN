---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd0722e81fd2af7b74b42d9fa91cd83841e6407e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let skills = await client.api('/me/profile/skills')
    .version('beta')
    .get();

```