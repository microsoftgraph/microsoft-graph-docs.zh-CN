---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91676f25f4ddccb6f140903e04a4d0ead83207ee
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/publications/{id}')
    .version('beta')
    .delete();

```