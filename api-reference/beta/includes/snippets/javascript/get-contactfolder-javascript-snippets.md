---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70c34177bafebffb55a8a763a4ae77c8bdf1901e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contactFolder = await client.api('/me/contactFolders/{id}')
    .version('beta')
    .get();

```