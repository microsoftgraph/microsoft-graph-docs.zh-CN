---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2823042aff92ec13858926c43cb3194c2abdd4af404ca1c01ef4c8c9703476bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333188"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBrandingLocalization = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr')
    .version('beta')
    .get();

```