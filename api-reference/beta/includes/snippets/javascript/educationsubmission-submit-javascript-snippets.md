---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4901a3d131bcb599ea05f5849bdc76b926811e97775c12d1e9c35fe8dc5fac4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163988"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11021/assignments/19002/submissions/850f51b7/submit')
    .version('beta')
    .post();

```