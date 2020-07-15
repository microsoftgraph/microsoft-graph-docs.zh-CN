---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a56c4d451bb0ef0074aecc64644aa626ee9a87e
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182')
    .version('beta')
    .get();

```