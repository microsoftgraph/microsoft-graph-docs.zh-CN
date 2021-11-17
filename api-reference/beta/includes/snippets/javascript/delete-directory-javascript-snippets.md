---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fbaa2f29616ecf2fea6678a8f17c417608df797f298a577a5cd5a1ce8839995
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164269"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb')
    .version('beta')
    .delete();

```