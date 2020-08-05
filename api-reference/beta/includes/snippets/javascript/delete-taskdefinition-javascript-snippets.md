---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2ab3f6ca9a6f3502b00491a07c2c3a4be304621
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565737"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/taskDefinitions/4c6a0f26-8e5d-4bf6-91e6-4a5731adec19')
    .version('beta')
    .delete();

```