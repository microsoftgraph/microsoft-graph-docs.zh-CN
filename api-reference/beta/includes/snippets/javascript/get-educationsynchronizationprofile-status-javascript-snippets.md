---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5e5057e8a0381c3b1a45c5dbed20e5020ddbbd4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612238"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/profileStatus')
    .version('beta')
    .get();

```