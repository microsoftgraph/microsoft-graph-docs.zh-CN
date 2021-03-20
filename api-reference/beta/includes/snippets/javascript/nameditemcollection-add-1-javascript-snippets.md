---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c9d18a9fd643d793f964d39271a55eb2dce3cc4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  name: 'test5',
  reference: '=Sheet1!$F$15:$N$27',
  comment: 'Comment for the named item'
};

await client.api('/me/drive/items/{id}/workbook/names/add')
    .version('beta')
    .post(workbookNamedItem);

```