---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5fa665bd7870b724f31caee0793ea2e30e7da2c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registeredUsers = await client.api('/devices/{id}/registeredUsers')
    .get();

```