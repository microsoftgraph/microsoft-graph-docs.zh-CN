---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75c7f07d638624c5e228e65cd2c77153344684c9926c758a78ccc768646bdd61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reject = {
  reason: 'busy'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject')
    .version('beta')
    .post(reject);

```