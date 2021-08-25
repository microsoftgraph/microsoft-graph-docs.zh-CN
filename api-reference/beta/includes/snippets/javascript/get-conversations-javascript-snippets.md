---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f7b263509562e452762d7915710bebf9ac21b644442f2344f36cfda7e8f2f67
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277454"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversations = await client.api('/groups/{id}/conversations')
    .version('beta')
    .get();

```