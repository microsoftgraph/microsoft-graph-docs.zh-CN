---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42b5d0d967de79d7b56b5930452733920e530f89af344ee7bac910609f85d6c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tables = await client.api('/me/drive/items/{id}/workbook/tables')
    .get();

```