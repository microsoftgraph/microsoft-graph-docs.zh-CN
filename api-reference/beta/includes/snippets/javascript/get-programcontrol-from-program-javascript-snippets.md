---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2021a16a44ef2a75abf1f5349351d056ab91589e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls')
    .version('beta')
    .get();

```