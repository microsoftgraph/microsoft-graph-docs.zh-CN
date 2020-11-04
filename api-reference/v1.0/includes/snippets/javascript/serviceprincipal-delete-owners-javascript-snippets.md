---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4f29fff9f05c30952de5c6f76aee41c16c15324
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903509"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/owners/{id}/$ref')
    .delete();

```