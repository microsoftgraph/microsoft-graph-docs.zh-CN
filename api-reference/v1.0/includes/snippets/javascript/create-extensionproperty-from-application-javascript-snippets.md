---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88c5741699d249aa2409c45ec7be64a368208323
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998971"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extensionProperty = {
    name: "extensionName",
    dataType: "string",
    targetObjects: [
        "Application"
    ]
};

let res = await client.api('/applications/{id}/extensionProperties')
    .post(extensionProperty);

```