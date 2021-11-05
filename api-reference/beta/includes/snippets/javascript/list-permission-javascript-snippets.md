---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c078094162a2142d1bb1ef612955617fa488f8d
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780958"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sites = await client.api('/sites?search=%7Bquery%7D')
    .version('beta')
    .get();

```