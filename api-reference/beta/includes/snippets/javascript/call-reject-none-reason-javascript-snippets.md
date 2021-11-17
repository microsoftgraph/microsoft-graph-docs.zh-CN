---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d213ccfd9ce00e54df40e8f43ef63cc3f9145d4532aa5beb5d065d7e2a46634
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reject = {
  reason: 'none'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject')
    .version('beta')
    .post(reject);

```