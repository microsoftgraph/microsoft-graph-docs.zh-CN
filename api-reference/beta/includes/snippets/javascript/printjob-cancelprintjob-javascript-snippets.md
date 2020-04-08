---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e6b86c0fb699439e35f38cc25b57949e54ec633
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42947564"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/jobs/{id}/cancelPrintJob')
    .version('beta')
    .post();

```