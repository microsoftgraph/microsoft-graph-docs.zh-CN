---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fce344732dc8697f92a5532a729877f96f97d919e99d7ef3be0e40de1669bb6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .delete();

```