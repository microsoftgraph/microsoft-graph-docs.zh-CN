---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e125924f79be794b3db3cf0c93c54f6f935e7f45
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/publications/{id}')
    .version('beta')
    .delete();

```