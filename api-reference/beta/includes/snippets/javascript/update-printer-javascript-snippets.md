---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6570d8eb82789bf8cb3cac8df995062f5ca20e6c409f2e51426e2db32cfa5eea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902384"
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

await client.api('/print/printers/{id}')
    .version('beta')
    .update(printer);

```