---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c01d67c9709d2a100db5ecf70544d1dc0d352781
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printerShare = {
  displayName: 'PrinterShare Name',
  'printer@odata.bind': 'https://graph.microsoft.com/v1.0/print/printers/{printerId}',
  allowAllUsers: false
};

await client.api('/print/shares/{printerShareId}')
    .update(printerShare);

```