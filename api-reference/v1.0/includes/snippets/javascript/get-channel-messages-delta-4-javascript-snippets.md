---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47eec3b2ec7e4f3ed3460caf5fc623ea7d53d2f1
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .get();

```