---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20efeab82b6cbb815ce17fad5d6ada7b04c42188
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .version('beta')
    .top(2)
    .get();

```