---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2385fb28fb5be78cad4c13b71e29ec7f4b725f4d
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR')
    .delete();

```