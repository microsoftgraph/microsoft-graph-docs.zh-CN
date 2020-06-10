---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a351d8c61aab05966672eadc4f0ac5415794fdd
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681525"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf')
    .version('beta')
    .get();

```