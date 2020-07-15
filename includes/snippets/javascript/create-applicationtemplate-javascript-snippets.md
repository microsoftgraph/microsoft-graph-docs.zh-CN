---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 890085fcd032808129b7f000c0254d9f08635729
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const applicationServicePrincipal = {
  displayName: "Contoso IWA App"
};

let res = await client.api('/applicationTemplates/8adf8e6e-67b2-4cf2-a259-e3dc5476c621/instantiate')
    .version('beta')
    .post(applicationServicePrincipal);

```