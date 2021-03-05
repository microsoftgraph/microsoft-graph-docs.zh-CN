---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daa593be778458fb8daedf344cf8eca8e641c2c2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extension = {
  '@odata.type': 'microsoft.graph.openTypeExtension',
  extensionName: 'Com.Contoso.Deal',
  companyName: 'Alpine Skis',
  dealValue: 1010100,
  expirationDate: '2015-07-03T13:04:00.000Z'
};

await client.api('/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions')
    .post(extension);

```