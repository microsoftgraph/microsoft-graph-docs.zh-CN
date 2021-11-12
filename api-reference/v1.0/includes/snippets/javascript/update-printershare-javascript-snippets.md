---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb518bcf68cb7b5f376baf232a3f4412d34626ce69e25a1ef2e1a3b28ebc0e45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902238"
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