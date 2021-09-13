---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 044aca5d4e1adf9d90a7229b2aa6d18eef509489283591bd29044e30bacfae52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277661"
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