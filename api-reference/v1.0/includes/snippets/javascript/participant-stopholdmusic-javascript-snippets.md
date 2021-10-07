---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 471b039e2596e7ce6f4df518ec64a67dbc0c86e1
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214619"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stopHoldMusicOperation = {
  clientContext: 'd45324c1-fcb5-430a-902c-f20af696537c',
};

await client.api('/communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/participants/fa1e9582-7145-4ca3-bcd8-577f561fcb6e/stopHoldMusic')
    .post(stopHoldMusicOperation);

```