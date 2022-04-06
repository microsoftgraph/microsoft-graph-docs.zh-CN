---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4668d1a56be669df38d24d85f608851436be1f0611ca5c0923afff1e18ca4e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332516"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore')
    .version('beta')
    .post();

```