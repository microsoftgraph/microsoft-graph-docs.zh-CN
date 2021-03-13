---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f11cc2b7de6cef5701d9f71377867b6fdee8ddc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783615"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{id}/unarchive')
    .version('beta')
    .post();

```