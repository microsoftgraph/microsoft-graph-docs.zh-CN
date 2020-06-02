---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df7411e593133bd324bb329ac79aa2190e0b855b
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216733"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printerShare = {
  name: "ShareName",
  printer@odata.bind: "https://graph.microsoft.com/beta/print/printers/{id}"
};

let res = await client.api('/print/shares/{id}')
    .version('beta')
    .update(printerShare);

```