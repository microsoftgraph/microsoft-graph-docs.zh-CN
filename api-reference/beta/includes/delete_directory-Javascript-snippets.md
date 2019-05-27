---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6ec76fd298c148a63250cc6a2bc71326c5256665
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438593"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb')
    .version('beta')
    .delete();

```