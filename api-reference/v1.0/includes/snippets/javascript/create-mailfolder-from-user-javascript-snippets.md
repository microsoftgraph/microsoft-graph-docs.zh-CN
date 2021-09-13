---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa4318a161029f72af9c8a204fc6466e07ba90f8d438e14282cf5811021e536c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103767"
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
    .post(mailFolder);

```