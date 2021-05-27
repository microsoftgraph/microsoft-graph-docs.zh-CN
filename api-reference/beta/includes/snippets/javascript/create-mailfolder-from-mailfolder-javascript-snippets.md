---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c43535aeceb53041ae20d2edf6bdb0fdf59a4776
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668759"
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