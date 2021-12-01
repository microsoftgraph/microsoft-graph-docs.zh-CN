---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8785b93d8e49dcb50c95ea4ad42bec597af9d23892ad2632b0b0dd5bd3730923
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220307"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissions = await client.api('/me/drive/items/{item-id}/permissions')
    .version('beta')
    .get();

```