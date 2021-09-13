---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57d874d6c54bf78c2051e0e829de755f04efa421af04a702d309c100ecc1db3f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/unsubscribeByMail')
    .post();

```