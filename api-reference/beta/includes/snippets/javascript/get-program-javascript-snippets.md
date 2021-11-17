---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73d0ee218a60d4a44493571c4953964f120a41d5513e3255074b11b0ffac31d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277761"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let programs = await client.api('/programs')
    .version('beta')
    .get();

```