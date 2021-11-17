---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 189d57ab30158bc51ed02d7b664659db86b38751907135c4059b96a0102fbd98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279619"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/termStore/sets/{setId}/children')
    .version('beta')
    .get();

```