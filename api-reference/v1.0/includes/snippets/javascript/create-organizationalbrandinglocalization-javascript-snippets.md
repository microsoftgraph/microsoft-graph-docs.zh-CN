---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a85a613efdc5d0c347dafb2fc62c5ad53ae8ee0
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996962"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBrandingLocalization = {
    backgroundColor: '#00000F',
    id: 'fr-FR',
    signInPageText: ' '
};

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations')
    .post(organizationalBrandingLocalization);

```