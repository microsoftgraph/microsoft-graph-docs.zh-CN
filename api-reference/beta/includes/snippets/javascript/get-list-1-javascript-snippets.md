---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9493327926ca87c9cac48df648481ffb111f9dee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958013"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{site-id}/lists/{list-id}')
    .version('beta')
    .get();

```