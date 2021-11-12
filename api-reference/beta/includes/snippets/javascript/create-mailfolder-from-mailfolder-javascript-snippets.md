---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9438fe1bfc15e40fd1d4c510846a9ce301286d560bc8531f2fcf02e14084c618
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219181"
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
    .version('beta')
    .post(mailFolder);

```