---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14b722f4af1685d28db4e7046cc8ed434da24532e2ec35b68b5b271161c49433
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331964"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let endpoints = await client.api('/groups/{id}/endpoints')
    .version('beta')
    .get();

```