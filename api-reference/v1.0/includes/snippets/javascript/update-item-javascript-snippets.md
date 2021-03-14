---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e85e1043341a0365a7fa70cb99320d651cea4b7c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790712"
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
    .update(driveItem);

```