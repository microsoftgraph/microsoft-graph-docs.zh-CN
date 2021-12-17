---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2597d613fdd8ce52d911c464e3256d5e1e3d9a87
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61544916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments')
    .version('beta')
    .expand('resources')
    .get();

```