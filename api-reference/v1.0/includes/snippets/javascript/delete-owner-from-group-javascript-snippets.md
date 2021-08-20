---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc6016f4a757744dbb222d7758eba491a0c8c08516413a5a5a8e8fba99ba5d74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/owners/{id}/$ref')
    .delete();

```