---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40435cef19895122e540e9dd8b1c480e4145037e
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730177"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/education/users/80cefd93-8d88-40e2-b5d3-67898383e226/assignments?expand=submissions')
    .version('beta')
    .get();

```