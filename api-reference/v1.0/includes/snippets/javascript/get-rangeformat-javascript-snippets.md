---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 511ffb8b47cbc1acc973dbb81a447a83107db4d67d8041750d2e1026a65f0ef1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeFormat = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format')
    .get();

```