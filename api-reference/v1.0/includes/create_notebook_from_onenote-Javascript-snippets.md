---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8a54a4dd1aa8936f330bdbe651f08b8c46f6b20e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460388"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const notebook = {
  displayName: "Notebook name"
};

let res = await client.api('/me/onenote/notebooks')
    .post({notebook : notebook});

```