---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cb59c813634b30a295ced5547537bbc7a725f26a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478130"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/addFavorite')
    .post();

```