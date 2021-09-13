---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7981d05cab63ec5d516c219d780a4d1fbdd751b5f40854b830fb30ecf53989d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904105"
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
    .update(place);

```