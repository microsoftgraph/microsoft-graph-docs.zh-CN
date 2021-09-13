---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7cefda68bbcc8c954a3ef60cc76163e931897b83acaa1a67311cdf3691a7851
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rows = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows')
    .get();

```