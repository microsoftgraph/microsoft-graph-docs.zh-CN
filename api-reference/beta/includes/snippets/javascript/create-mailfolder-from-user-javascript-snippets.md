---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3adbdb75ee8dd86bf3708febefc9b01ad59df6931fc1bfac6e9feb9bf2ee6360
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279609"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: 'Clutter',
  isHidden: true
};

await client.api('/me/mailFolders')
    .version('beta')
    .post(mailFolder);

```