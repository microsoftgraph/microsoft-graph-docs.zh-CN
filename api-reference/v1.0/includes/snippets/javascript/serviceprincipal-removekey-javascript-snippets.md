---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d6b69b2d6fd035974611ef18aa1ca4326e885e520f1147416adbfe85b90e35a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219998"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removeKey = {
    keyId: 'f0b0b335-1d71-4883-8f98-567911bfdca6',
    proof: 'eyJ0eXAiOiJ...'
};

await client.api('/servicePrincipals/{id}/removeKey')
    .post(removeKey);

```