---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fde6f7cc92bc8a6a60ca22a5ba68c48be7f87fbb
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905619"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/transitiveMemberOf')
    .get();

```