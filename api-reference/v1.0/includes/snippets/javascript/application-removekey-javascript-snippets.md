---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35620ffc3225811a396b69eb01424328ccc3737d8839470d89f9c4cc11f4bb1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902343"
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

await client.api('/applications/{id}/removeKey')
    .post(removeKey);

```