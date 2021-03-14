---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b40ec0751e759a3a2ad0102dd2b1826844decefd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810371"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/conditionalAccess/policies/{id}')
    .delete();

```