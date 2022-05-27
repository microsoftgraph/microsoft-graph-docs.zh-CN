---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6975111a24320e9b3cd728bd3805a07d57ddd74baed011b6faa27ecc4d120177
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/shares/{id}/allowedGroups/{id}/$ref')
    .version('beta')
    .delete();

```