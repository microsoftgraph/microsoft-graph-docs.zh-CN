---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1f32d854bf103e27da0ebaaf2e68ec7b30c6f6c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: 'Volunteer'
};

await client.api('/me/calendars')
    .post(calendar);

```