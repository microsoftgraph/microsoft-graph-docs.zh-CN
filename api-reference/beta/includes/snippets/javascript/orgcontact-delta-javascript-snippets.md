---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ad612cd3071101cad923c0da271b1c78de30398004707b91979bef6b1de2576
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .version('beta')
    .get();

```