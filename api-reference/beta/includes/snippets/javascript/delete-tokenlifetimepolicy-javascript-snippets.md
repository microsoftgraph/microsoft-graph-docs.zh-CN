---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d6e2f79b9337b25d18c324cc7db676a1fa73775
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenLifetimePolicies/{id}')
    .version('beta')
    .delete();

```