---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90bfa27e3d0afd5528034969bcfde51ae366b3d2
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758592"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0'
};

await client.api('/users/10f17b99-784c-4526-8747-aec8a3159d6a/manager/$ref')
    .put(directoryObject);

```