---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eef0916e05f64428901fe7552f6db6ebd5459d7d1db5941170e59941046af5b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161297"
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
    .version('beta')
    .post(removeKey);

```