---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8596d032b6ed19bb0ebe2ed9e43813368e9f0a72246d547c05e9a6042bac1050
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904045"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/resetUnseenCount')
    .version('beta')
    .post();

```