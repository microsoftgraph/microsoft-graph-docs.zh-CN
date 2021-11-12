---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c8e776e4f79fb0a2dea9cbf8c91dc25d3a1cbe110a29e5a012bfc7158598ba3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let borders = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders')
    .version('beta')
    .get();

```