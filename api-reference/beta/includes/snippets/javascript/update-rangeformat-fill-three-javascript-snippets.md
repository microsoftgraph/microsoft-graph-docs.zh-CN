---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5560824409f2a9e8291f68bc2a067dce826241755a8d06604ab7b8cd72c21810
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106302"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: '#0000FF'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill')
    .version('beta')
    .update(workbookRangeFill);

```