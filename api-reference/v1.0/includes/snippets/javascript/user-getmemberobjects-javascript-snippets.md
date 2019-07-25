---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f72eb07fd37e1441f7a2da3be7fd7660ab3bc167
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714871"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/me/getMemberObjects')
    .post(String);

```