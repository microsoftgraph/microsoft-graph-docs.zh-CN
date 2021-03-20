---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e48c722b6d61e027e161432fd42d87ddbd4fec6e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945065"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shares = await client.api('/print/shares')
    .get();

```