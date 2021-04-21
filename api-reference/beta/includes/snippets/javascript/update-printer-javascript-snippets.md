---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f9aa72705d0b3036c64ff0ac2cc988511edb5fb
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921985"
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