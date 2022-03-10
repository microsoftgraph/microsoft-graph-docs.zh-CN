---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb5759d0808514a55832310b14e29dc81b3cc05b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412478"
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
    .post(extensionProperty);

```