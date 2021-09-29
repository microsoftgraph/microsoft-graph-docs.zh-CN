---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7ff39b7c72cc2413c6c053c9247c025d431995a
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBrandingLocalization = {
    backgroundColor: '#00000F',
    signInPageText: 'Welcome to Contoso France'
};

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR')
    .version('beta')
    .update(organizationalBrandingLocalization);

```