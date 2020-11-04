---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5872b7a26e66f6dfb7a69aaf0a5de06b7e9136d9
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904191"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/unfollow')
    .post();

```