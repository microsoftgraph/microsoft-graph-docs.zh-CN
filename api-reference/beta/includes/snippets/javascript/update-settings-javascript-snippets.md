---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 359920d31c8bc74897b6ecf641530931d39ae8e1
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printSettings = {
  documentConversionEnabled: true
};

let res = await client.api('/print/settings')
    .version('beta')
    .update(printSettings);

```