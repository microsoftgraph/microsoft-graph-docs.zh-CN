---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 613b1fe1518b0aa3f799014c884e890cef438ed29dd99496a1d52b073ac18f00
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220131"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
    'groupIds-value'
  ]
};

await client.api('/me/checkMemberGroups')
    .post(string);

```