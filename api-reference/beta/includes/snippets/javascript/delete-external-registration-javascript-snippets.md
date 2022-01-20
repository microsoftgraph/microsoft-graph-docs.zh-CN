---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2424fed2dd9e7011ed8a4177cc922c386b7e9db2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113579"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration')
    .version('beta')
    .delete();

```