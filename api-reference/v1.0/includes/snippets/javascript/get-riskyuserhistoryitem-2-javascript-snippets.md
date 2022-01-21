---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e30871b459e21f375a11af3cac854b2a8c8ae7d5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091855"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let history = await client.api('/identityProtection/riskyUsers/{riskyUserId}/history')
    .get();

```