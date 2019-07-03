---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b1e2d9655e2fb2808d176a9a6109c303214a71f0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479877"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programControls')
    .version('beta')
    .get();

```