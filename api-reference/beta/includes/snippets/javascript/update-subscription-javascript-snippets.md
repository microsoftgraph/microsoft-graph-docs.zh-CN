---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 381409ec053f918f5c473633aec237281cb4a8ff
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636679"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscription = {
   expirationDateTime:"2016-11-22T18:23:45.9356913Z"
};

let res = await client.api('/subscriptions/{id}')
    .version('beta')
    .update(subscription);

```