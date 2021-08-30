---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b242f375e2a35f37b0b4d2b35080b5f2b5e51a157a687559c947f410b35d56c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let application = await client.api('/applications/{id}')
    .version('beta')
    .get();

```