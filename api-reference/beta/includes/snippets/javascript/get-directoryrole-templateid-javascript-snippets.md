---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5f1dbbb2eaf7c5ad6479249c42b0ab8b6e61f91
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991717"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRole = await client.api('/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b')
    .version('beta')
    .get();

```