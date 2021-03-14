---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d88881286dac2399dc1c248dc1b73e04d7f56a63
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804336"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const changeScreenSharingRole = {
  role: 'viewer'
};

await client.api('/communications/calls/{id}/changeScreenSharingRole')
    .post(changeScreenSharingRole);

```