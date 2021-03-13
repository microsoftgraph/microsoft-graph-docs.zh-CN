---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31fce9f15fd46b282ab6902fe85cb5e3ec2ca0bc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printerShare = {
  name: 'ShareName',
  'printer@odata.bind': 'https://graph.microsoft.com/beta/print/printers/{id}'
};

await client.api('/print/shares/{id}')
    .version('beta')
    .update(printerShare);

```