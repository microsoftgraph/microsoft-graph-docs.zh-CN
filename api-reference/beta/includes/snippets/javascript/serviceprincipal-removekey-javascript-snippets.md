---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2321a9d296cbd10fdf3900e76a2777a325ab38e623487b5972c06e687802e308
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274126"
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

await client.api('/serviceprincipals/{id}/removeKey')
    .version('beta')
    .post(removeKey);

```