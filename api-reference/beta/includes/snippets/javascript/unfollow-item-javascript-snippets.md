---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b49b0d16d055e101b27a0b0c4b61c0aa069c04d2
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61228319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}/unfollow')
    .version('beta')
    .post();

```