---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e1639a153957ca0926b1b458571db5cce23b897
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782893"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  parentFolderId: 'parentFolderId-value',
  displayName: 'displayName-value'
};

await client.api('/me/contactFolders/{id}')
    .version('beta')
    .update(contactFolder);

```