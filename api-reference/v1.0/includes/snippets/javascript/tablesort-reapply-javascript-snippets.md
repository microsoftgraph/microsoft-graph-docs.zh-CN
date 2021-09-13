---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39eebef7c5f9e54af553e92cf643fbcf85a64402f6cc099eb2f1556df83ab584
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply')
    .post();

```