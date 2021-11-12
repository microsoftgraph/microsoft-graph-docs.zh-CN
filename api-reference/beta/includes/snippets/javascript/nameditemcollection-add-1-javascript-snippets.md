---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e26ff793b4a63085232b5874849e0015baded1dd23fb117a225661ecb0e0d55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106004"
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