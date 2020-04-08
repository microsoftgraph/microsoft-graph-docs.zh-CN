---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb8968947ff50bb0827ca713765172673c135a29
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948088"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/jobs/{id}/documents/{id}/uploadData')
    .version('beta')
    .post();

```