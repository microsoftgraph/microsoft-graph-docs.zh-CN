---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bf753b660ca48e00f98b8de2d0ad6ab2d3630216
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/invalidateAllRefreshTokens')
    .version('beta')
    .post();

```