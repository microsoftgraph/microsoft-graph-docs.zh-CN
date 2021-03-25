---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa6c0a8b0b667df11f97222e0a5b0483b88840c4
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210610"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .top(2)
    .get();

```