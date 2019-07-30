---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 130cf43170a4f2c2529c4827a4e220d604bb4630
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932664"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/bundles')
    .version('beta')
    .get();

```