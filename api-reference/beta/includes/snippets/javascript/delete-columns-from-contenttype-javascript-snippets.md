---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c338765da57b45b52b22779d8b63b8ea0b40b0c7451db8fc6dbb9b1ae15afd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161891"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}')
    .version('beta')
    .delete();

```