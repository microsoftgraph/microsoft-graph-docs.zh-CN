---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdc0d9ca05500c2b8f1b06bae77442dd8d8d47000eadd2b11036ff92e641e38f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163932"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  id: 'id-value',
  color: 'color-value',
  style: 'style-value',
  sideIndex: 'sideIndex-value',
  weight: 'weight-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders')
    .version('beta')
    .post(workbookRangeBorder);

```