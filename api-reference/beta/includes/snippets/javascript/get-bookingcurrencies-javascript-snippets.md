---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96cd8ac3d3032dff68406b3b3e0207ae1f176f67dbc9fe4fc86d571b2b26b4e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105037"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingCurrencies = await client.api('/bookingCurrencies')
    .version('beta')
    .get();

```