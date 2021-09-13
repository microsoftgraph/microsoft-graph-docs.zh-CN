---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e7c96969e0f356f9a9cdfae35cca3cab4c335d33688dc81739da2404fc44786
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219084"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const refreshSession = {

};

await client.api('/me/drive/items/{id}/workbook/refreshSession')
    .post(refreshSession);

```