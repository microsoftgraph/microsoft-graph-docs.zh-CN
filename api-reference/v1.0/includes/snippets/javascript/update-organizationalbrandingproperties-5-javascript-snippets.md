---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e96ce5a2f9d897aeb1fb978e39ac73a0b0237d7d80fa736e0e5890f6ea8231f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = <Image>;

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo')
    .put(stream);

```