---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08763e335ff7385ac6302fa219457095aa520b0f76131b810045b426c54fe55e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment')
    .version('beta')
    .post();

```