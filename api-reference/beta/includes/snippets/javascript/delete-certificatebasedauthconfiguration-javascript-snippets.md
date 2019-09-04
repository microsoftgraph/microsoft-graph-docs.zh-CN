---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cf794a19831428f25032dd814dd68c1da7fd7b0c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization/{id}/certificateBasedAuthConfiguration/{id}')
    .version('beta')
    .delete();

```