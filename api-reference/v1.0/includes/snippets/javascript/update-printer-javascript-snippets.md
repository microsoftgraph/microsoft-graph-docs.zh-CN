---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 384195e58376a7d965ba52d43d67e6463cf6385324e1571706a0b2d91c48941c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158335"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printer = {
  name: 'PrinterName',
  location: {
    latitude: 1.1,
    longitude: 2.2,
    altitudeInMeters: 3
  }
};

await client.api('/print/printers/{printerId}')
    .update(printer);

```