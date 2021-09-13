---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea5d4a4fdd8eb2ef5bc2aaa8c3f2debf4c9c89bc63eff8d31d4c5aef1bbecdcf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let series = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series')
    .get();

```