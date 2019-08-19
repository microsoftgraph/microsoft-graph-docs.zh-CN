---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 20f0d353631ac08b4ea8c42143c0e213a017e7d3
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460992"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/rubrics/{id}')
    .version('beta')
    .get();

```