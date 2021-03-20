---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 058b058c916b5671dacd9f9c55f85ba3f46e966f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943932"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBranding = {
    backgroundColor: '#FFFF33'
};

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding')
    .version('beta')
    .put(organizationalBranding);

```