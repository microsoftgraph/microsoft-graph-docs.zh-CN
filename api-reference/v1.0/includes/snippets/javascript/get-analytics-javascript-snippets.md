---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24a5d2bda7d90a0d4f04b0d24f3f128c7a1c269e2faf9d679150e866440cf55b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903891"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemAnalytics = await client.api('/drives/{drive-id}/items/{item-id}/analytics')
    .get();

```