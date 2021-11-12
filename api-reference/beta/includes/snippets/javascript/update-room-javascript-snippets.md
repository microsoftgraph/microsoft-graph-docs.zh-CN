---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcc2dd573a05b0659cb9c828bd7672440d1a4b05c1d7f41df624d50b76e4608e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const place = {
  '@odata.type': 'microsoft.graph.room',
  nickname: 'Conf Room',
  building: '1',
  label: '100',
  capacity: 50,
  isWheelChairAccessible: false
};

await client.api('/places/cf100@contoso.com')
    .version('beta')
    .update(place);

```