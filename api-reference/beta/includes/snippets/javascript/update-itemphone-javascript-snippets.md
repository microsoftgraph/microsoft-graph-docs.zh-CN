---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 627ff3e60c0dc639709a94885e21781b4fc2362e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPhone = {
  type: 'other'
};

await client.api('/users/{userId}/profile/phones/{id}')
    .version('beta')
    .update(itemPhone);

```