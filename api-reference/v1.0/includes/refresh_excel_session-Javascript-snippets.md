---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f74bb9512041406fdb5a6506b24e0d9cd0a39845
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const refreshSession = {

};

let res = await client.api('/me/drive/items/{id}/workbook/refreshSession')
    .post(refreshSession);

```