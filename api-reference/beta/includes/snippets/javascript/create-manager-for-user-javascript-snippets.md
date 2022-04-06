---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e45b3657ad7020853110ed7677b603887d9f491
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759033"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    '@odata.id': 'https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0'
};

await client.api('/users/10f17b99-784c-4526-8747-aec8a3159d6a/manager/$ref')
    .version('beta')
    .put(directoryObject);

```