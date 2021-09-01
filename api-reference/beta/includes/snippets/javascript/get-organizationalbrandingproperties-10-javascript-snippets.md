---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d7eb3ea110c4b8d29356b0099c0baf7b2c8639016b268812555a3174971c9be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279277"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let string = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText')
    .version('beta')
    .get();

```