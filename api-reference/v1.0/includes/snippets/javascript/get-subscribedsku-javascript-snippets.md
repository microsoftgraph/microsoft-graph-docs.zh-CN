---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f755bb8f22e3c9ae7130b96bd68db8d10717adaad74cbf5d99a56cf7b6b1f77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscribedSku = await client.api('/subscribedSkus/{id}')
    .get();

```