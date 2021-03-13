---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e14eb8137d0712d47da05eba8f6717ced6cede40
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printConnector = await client.api('/print/connectors/{id}')
    .version('beta')
    .get();

```