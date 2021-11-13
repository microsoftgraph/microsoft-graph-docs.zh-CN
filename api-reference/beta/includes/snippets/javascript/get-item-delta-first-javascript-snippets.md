---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eed4f824cd65820f55fe5ac05d037a44e43aa9803ae3eec4204c5d40b1c2b1ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/drive/root/delta')
    .version('beta')
    .get();

```