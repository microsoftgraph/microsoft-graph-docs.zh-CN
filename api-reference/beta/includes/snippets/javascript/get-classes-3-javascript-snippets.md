---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24dfcee1598dbbb12c4daf0611c1498f3e2f9867
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let classes = await client.api('/education/me/classes')
    .version('beta')
    .get();

```