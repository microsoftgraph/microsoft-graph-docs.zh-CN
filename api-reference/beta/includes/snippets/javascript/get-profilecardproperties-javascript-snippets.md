---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bb0fd4c609b21c1e25fcb3ea319fe81e0772915
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization/settings/profileCardProperties')
    .version('beta')
    .get();

```