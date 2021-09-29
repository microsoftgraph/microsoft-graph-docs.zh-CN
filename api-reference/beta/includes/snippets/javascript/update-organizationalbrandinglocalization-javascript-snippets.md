---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b56978b237f8e3493c20f99876e88f2c0be458bd
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996576"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = <Image>;

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR/bannerLogo')
    .version('beta')
    .put(stream);

```