---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e84524e23b4b7f91bed3a25151d60f6ae189c4c0a33f2b6fa1565f8aa11dd6b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}')
    .delete();

```