---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f43cb52b60afdd2870d1196f2dee7668164f500e725f953af79e8c8ad86cbf49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106309"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  italic: true,
  size: 26
};

await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font')
    .version('beta')
    .update(workbookRangeFont);

```