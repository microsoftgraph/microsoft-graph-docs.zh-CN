---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8273b3a6cebf069bc51cdd0fcf5b9448cadecf32e8021d13169047d66dd4d15f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279456"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const refreshSession = {

};

await client.api('/me/drive/items/{id}/workbook/refreshSession')
    .version('beta')
    .post(refreshSession);

```