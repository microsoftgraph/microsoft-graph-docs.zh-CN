---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5300ecda0fe5ebee9c536734a399d86f0c2a133f0282028936c72593860aeec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/addFavorite')
    .version('beta')
    .post();

```