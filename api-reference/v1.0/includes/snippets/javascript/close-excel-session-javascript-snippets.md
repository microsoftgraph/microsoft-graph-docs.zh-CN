---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a9bfb81501ab6532202c9ec026f494defc7c9570293e718ffe9289c3da8baa2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220957"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const closeSession = {

};

await client.api('/me/drive/items/{id}/workbook/closeSession')
    .post(closeSession);

```