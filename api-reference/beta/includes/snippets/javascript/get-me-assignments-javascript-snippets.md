---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4088e7da33cd2e1b380f3cbe8c45bbf125394d9d
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/education/me/assignments')
    .version('beta')
    .get();

```