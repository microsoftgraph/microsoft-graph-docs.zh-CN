---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6895be6b1e7cb35aad7a1bfbc7b2b08efe93eb9938ec05844767ea203a8fd4c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/contacts')
    .header('ConsistencyLevel','eventual')
    .search('displayName:wa')
    .get();

```