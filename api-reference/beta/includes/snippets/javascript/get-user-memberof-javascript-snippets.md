---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ab0a336336dadbc92526620ab15ab2787b4a3f1e9d4fc6dc21e8d75970620b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/users/{id}/memberOf')
    .version('beta')
    .get();

```