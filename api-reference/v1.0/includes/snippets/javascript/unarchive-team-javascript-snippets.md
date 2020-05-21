---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af1b2f32f67078e9555fadb241cb53b60903d5c2
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/unarchive')
    .post();

```