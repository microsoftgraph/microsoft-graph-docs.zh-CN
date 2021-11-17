---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d93c17a7c32a4640f55c8bf2bcb6649dd1e08bc28a1d4b4a3f0c7a9ea52703a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104434"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extensionProperty = {
    name: 'extensionName',
    dataType: 'string',
    targetObjects: [
        'Application'
    ]
};

await client.api('/applications/{id}/extensionProperties')
    .version('beta')
    .post(extensionProperty);

```