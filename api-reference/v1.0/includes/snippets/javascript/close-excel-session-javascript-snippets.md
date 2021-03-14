---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4c9d3df51bd6da68df18fd3e6e540795f6352f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792668"
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