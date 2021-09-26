---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ad48212ecd33a3628de6e48b8e810ec602c041aee80e8f0f717b96408ed4640
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/users/{id}/transitiveMemberOf')
    .version('beta')
    .get();

```