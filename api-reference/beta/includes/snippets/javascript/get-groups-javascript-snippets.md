---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 944e3637d99e6bc15e591c526d00e5ce41b54f864577d8c7214ec09b8341cff7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/groups')
    .version('beta')
    .get();

```