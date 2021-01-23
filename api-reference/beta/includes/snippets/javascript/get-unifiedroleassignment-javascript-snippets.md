---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af56978d8924b55bf376916ad56dfec61e790f7a
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946143"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1')
    .version('beta')
    .expand('directoryScope')
    .get();

```