---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1012a826ba018d73e89f9a46da40a5c0cc954eff6be320968091c763121cec99
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo')
    .header('Accept-Language','de')
    .get();

```