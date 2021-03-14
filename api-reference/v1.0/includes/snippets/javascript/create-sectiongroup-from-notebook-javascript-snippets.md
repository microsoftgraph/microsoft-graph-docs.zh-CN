---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad327c62d08cce3df932a41fe7c189b184bd7398
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801228"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: 'Section group name'
};

await client.api('/me/onenote/notebooks/{id}/sectionGroups')
    .post(sectionGroup);

```