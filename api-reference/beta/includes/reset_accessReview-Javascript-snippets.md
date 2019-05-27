---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a1809ec3bf0a8b5e8424868ec049c3ac34ae248d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions')
    .version('beta')
    .post();

```