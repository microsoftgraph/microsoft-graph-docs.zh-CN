---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32a16388e17605ec9f085b537a68f4d0ed9b58d16b0826dd9119123dddfe0d87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/shares/{printerShareId}/jobs/{printJobId}/start')
    .post();

```