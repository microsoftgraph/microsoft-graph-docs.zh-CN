---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84954dd09652b422eaaddd134d59a9f2c8eea578
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944022"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo')
    .version('beta')
    .header('Accept-Language','de')
    .get();

```