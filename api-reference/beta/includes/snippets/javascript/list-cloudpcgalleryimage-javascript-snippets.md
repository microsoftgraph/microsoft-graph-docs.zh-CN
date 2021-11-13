---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44ee4a5417573a997b7e661c7f767a1205a41bbb
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890467"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let galleryImages = await client.api('/deviceManagement/virtualEndpoint/galleryImages')
    .version('beta')
    .get();

```