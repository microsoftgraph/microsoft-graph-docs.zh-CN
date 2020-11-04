---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 319d96d08a8cb647e3551f2f7657d5e10b6e1382
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905017"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .top(2)
    .get();

```