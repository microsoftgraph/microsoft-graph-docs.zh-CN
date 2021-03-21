---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c94bba4d54dd2903928f9e62a97b24e7c1eb6e20
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959725"
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