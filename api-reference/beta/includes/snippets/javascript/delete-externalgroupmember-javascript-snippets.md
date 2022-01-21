---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40ab2bf6f0ba08416433839d1b73ccea1d65377f49f1e9701770092aad9bfc3f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a')
    .version('beta')
    .delete();

```