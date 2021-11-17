---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e86ff2583e2d488a201502172d71fb17ba1c1a3f42b03501b468f6e52518288
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220589"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sites = await client.api('/sites')
    .version('beta')
    .filter('siteCollection/root ne null')
    .select('siteCollection,webUrl')
    .get();

```