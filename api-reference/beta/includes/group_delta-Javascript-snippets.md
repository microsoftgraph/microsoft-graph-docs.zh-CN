---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1a7a9fd8404184ee96bf74c469bd7f7519978589
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444774"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/delta')
    .version('beta')
    .header('Prefer','return=minimal')
    .select('displayName,description,mailNickname')
    .get();

```