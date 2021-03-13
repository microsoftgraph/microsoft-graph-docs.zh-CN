---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f3007c4c380e76498140d844ec6715ea92fb1ee
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798176"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let projects = await client.api('/me/profile/projects')
    .version('beta')
    .get();

```