---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 687c57cda69cb57e0ff84035550e8c9cc5e7f995f35f8e49de913b1b9801d2c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219417"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let entries = await client.api('/admin/windows/updates/catalog/entries')
    .version('beta')
    .get();

```