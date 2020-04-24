---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c68065cbe4f0da0803a6e12c786c6a814f9afc8
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806515"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/authentication/passwordMethods/{id}')
    .version('beta')
    .get();

```