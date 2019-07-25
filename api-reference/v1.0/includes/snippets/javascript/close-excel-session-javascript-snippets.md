---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a1d7ec71ec175b4717532b5774ca3397b51dc0d7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const closeSession = {

};

let res = await client.api('/me/drive/items/{id}/workbook/closeSession')
    .post(closeSession);

```