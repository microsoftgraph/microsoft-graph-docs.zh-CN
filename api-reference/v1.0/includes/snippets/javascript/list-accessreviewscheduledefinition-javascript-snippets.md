---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc71c8763d82d0d30dfa1feb911818d06433065c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208705"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let definitions = await client.api('/identityGovernance/accessReviews/definitions')
    .skip(0)
    .top(100)
    .get();

```