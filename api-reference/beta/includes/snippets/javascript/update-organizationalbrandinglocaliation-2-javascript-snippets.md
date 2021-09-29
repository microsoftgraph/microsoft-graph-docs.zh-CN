---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3402dbc5336b91d489b9d667fcf56838a186d32c
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995568"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = <Image>;

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo')
    .version('beta')
    .update(stream);

```