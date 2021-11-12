---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ac6ca57870e1cca4e227b6bacf9c0c9c404502a12dd8abe39c54d284b21159f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allowedGroups = await client.api('/print/shares/{id}/allowedGroups')
    .version('beta')
    .get();

```