---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02ab7d49626c9995009871f558ff880c236554b6
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476800"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenLifetimePolicies/{id}')
    .version('beta')
    .get();

```