---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6c403b06cb89d6daaf5d9d023820d825e46032e9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436353"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/delta')
    .version('beta')
    .get();

```