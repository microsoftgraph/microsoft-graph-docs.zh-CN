---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca91c8911d0132e2ffb1fd460b3d98f9dbbd1e3f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961203"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/tokenLifetimePolicies/{id}/appliesTo')
    .get();

```