---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91021246311133868ef282cba2e6b25bd205cb5d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
  displayName: 'MSGraph Sample',
  isViewingBeforeAcceptanceRequired: true,
  files: [
    {
      fileName: 'TOU.pdf',
      language: 'en',
      isDefault: true,
      fileData: {
        data: 'SGVsbG8gd29ybGQ='
      }
    }
  ]
};

await client.api('/identityGovernance/termsOfUse/agreements')
    .version('beta')
    .post(agreement);

```