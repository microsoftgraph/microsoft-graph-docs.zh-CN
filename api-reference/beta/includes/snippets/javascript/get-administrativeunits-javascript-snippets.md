---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a273d9e16fbfecd2c73997ced3c505684539a91
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608350"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/administrativeUnits')
    .version('beta')
    .get();

```