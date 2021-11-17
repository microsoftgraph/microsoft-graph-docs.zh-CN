---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f324e643f4982b07253fae93c445168ac8b2ec76b48e24bea3c126b6c03a61e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273988"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/languages/{id}')
    .version('beta')
    .delete();

```