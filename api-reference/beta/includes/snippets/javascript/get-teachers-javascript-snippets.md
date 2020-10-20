---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a6cae59e36d3aec710e4c3c4f7a0a261ddc8d91
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620800"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11023/teachers')
    .version('beta')
    .get();

```