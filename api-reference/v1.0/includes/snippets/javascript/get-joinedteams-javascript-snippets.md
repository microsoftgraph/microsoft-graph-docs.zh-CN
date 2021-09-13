---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddf8352ee8a05da6577b4fb5a31cc8bcd76c5dc9bf07611d8092ef5ce2016dce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let joinedTeams = await client.api('/me/joinedTeams')
    .get();

```