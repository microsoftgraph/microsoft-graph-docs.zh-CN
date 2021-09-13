---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3be456698b2623cd22af3a324db956c3c790f6c8a526ec17635c2248f2b6283c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904138"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/domains/contoso.com')
    .delete();

```