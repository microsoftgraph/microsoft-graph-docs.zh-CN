---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2124ebf40f3bae094a01335ed9a67114c6751b51
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42947561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/services/{id}')
    .version('beta')
    .get();

```