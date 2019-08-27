---
description: 自动生成的文件。 不修改
ms.openlocfilehash: acdc26bca4ab9671b6e078f8ada82bd2c6a8d364
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636526"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "new-file-name.docx"
};

let res = await client.api('/me/drive/items/{item-id}')
    .version('beta')
    .update(driveItem);

```