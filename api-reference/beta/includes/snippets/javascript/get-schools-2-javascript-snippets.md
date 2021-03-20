---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d931ee85e38780f338c13aa0a1cc5de64840f9a8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951431"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schools = await client.api('/education/schools')
    .version('beta')
    .get();

```