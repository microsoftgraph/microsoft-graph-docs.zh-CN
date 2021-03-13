---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef438b8d810a826ca336422df676bb0e0bbebdb4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/me/contactFolders/{id}/contacts')
    .version('beta')
    .get();

```