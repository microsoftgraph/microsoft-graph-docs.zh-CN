---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b674d941b868fe9440da9fea42c5d83b1b1adbd3eb8533ff48377be66569856
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: 'edit',
  scope: 'organization'
};

await client.api('/me/drive/items/{item-id}/createLink')
    .post(permission);

```