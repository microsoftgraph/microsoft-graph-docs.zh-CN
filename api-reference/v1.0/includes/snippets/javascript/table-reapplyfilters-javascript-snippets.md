---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d3cb57bdadf5d26ccb7ef1d8f97b40cf69cf4f6108871b09c322483a75f9300
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158688"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters')
    .post();

```