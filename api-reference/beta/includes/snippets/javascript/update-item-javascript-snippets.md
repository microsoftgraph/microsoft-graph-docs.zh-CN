---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f1fbcc70969c4e2a5e6517c9c321d342f124d1b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799515"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: 'new-file-name.docx'
};

await client.api('/me/drive/items/{item-id}')
    .version('beta')
    .update(driveItem);

```