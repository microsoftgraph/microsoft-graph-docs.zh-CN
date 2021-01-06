---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02a3fb3e7cab184f4e5788b203183e5fb33fc004
ms.sourcegitcommit: df0778a4dbd1e7a2fde1846bdfbfd9440fc91672
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768661"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "Clutter",
  isHidden: true
};

let res = await client.api('/me/mailFolders')
    .version('beta')
    .post(mailFolder);

```