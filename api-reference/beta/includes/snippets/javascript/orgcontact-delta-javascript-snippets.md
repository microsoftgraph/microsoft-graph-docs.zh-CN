---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c620e9a43757ab5f3f570591134ca8524abf530
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/delta')
    .version('beta')
    .get();

```