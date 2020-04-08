---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f06cdfe2f7d317050678b3eec8b2d7773e1cd3a
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948173"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/connectors/{id}')
    .version('beta')
    .delete();

```