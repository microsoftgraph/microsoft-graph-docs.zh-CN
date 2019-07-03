---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2732d023798b4af955503939406d485fd104fef7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520971"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryroles/{id}/members/{id}/$ref')
    .version('beta')
    .delete();

```