---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: faa7c18baa203bbb434d78bec3cf5868db6dea28
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44052281"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/followedSites')
    .version('beta')
    .post();

```