---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 965904ad05bc682df8123ca2c0a2975ea2bdc150
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123636"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments')
    .version('beta')
    .get();

```