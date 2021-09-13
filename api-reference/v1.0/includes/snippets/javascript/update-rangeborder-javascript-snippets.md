---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe084dd49677d0a42fd1335a1470eddc02b61d372beece2bff80c6321d032d3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  color: 'color-value',
  style: 'style-value',
  sideIndex: 'sideIndex-value',
  weight: 'weight-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}')
    .update(workbookRangeBorder);

```