---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac2488031b39e13675f7ccd0af788eae1a6ff3c6
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948284"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printerShares')
    .version('beta')
    .get();

```