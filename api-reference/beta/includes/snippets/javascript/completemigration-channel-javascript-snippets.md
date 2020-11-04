---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68a7ce59516da5d82b9700a0bd04bda223e02e1f
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903967"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/channels/{channelId}/completeMigration')
    .version('beta')
    .post();

```