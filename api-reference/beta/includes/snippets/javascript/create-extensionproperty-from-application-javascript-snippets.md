---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c6fc22f3ebcc41381e82cd1072f7ee7f8138b7c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extensionProperty = {
    name: 'jobGroup',
    dataType: 'String',
    targetObjects: [
        'User'
    ]
};

await client.api('/applications/fd918e4b-c821-4efb-b50a-5eddd23afc6f/extensionProperties')
    .version('beta')
    .post(extensionProperty);

```