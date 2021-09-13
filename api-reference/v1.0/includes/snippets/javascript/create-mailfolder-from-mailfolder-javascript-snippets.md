---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3eda72241599ecc79f8f2f9ea9328cecbdc4ed7e1225d9f229d7ba12ee1a07c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279332"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: 'displayName-value',
  isHidden: true
};

await client.api('/me/mailFolders/{id}/childFolders')
    .post(mailFolder);

```