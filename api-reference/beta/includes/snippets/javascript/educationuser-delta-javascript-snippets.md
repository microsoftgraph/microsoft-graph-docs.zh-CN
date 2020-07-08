---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bd79390c2e5e79f47a8568115b3d64ec3ade764
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/users/delta')
    .version('beta')
    .get();

```