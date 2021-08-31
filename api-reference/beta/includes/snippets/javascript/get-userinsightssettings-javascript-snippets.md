---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21c3ef689f4b644ca19a02687b9e3d5c4d64476651a6dc6a3dbd3f94a0997e48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userInsightsSettings = await client.api('/me/settings/itemInsights')
    .version('beta')
    .get();

```