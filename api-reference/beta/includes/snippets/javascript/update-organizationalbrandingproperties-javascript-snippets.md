---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89b8a70d7d6ac724777ad77ac63f2664bff28387
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179499"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBranding = {
    backgroundColor:"#FFFF33"
};

let res = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding')
    .version('beta')
    .put(organizationalBranding);

```