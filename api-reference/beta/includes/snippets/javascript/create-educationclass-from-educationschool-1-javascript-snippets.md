---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13f7a185b7ee138ecc705a36299db0dec3112cc3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951667"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11003/members/14008')
    .version('beta')
    .delete();

```