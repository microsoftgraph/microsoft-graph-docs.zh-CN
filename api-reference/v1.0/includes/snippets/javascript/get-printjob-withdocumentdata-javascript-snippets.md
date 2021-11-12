---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa3095dac2c2b256f27697a3d8c02914882729fbeb86107d54bd522cc1fcb33b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162010"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printJob = await client.api('/print/printers/{printerId}/jobs/{printJobId}')
    .expand('documents')
    .get();

```