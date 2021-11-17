---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f43d42f4d8ae78209cb8f87ff7c97fd8a1eddbb41930fa9076fb5f23a3a4557
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/termStore/sets/{setId}')
    .version('beta')
    .delete();

```