---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60d9deb9065f427e60996dba9fd99a99aa0b200f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/synchronizationProfiles/{id}/pause')
    .version('beta')
    .post();

```