---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73298b80c589ad695c91d725f2e8e52f7f96cfcd3c473f24d02e4546274ad14b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273868"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/notebooks/{id}/sections')
    .version('beta')
    .get();

```