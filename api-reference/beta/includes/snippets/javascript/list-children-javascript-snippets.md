---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79191129d89b79c306ccd86785312d1effe59ed8fa5b69eab12fa7725ad339e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/drives/{drive-id}/items/{item-id}/children')
    .version('beta')
    .get();

```