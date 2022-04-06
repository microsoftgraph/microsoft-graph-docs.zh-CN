---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c832bc601bb74cf6faec23fbdf13da81db97493e
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
  displayName: 'Contoso ToU for guest users',
  isViewingBeforeAcceptanceRequired: true,
  files: [
    {
      fileName: 'TOU.pdf',
      language: 'en',
      isDefault: true,
      fileData: {
        data: 'SGVsbG8gd29ybGQ=//truncated-binary'
      }
    }
  ]
};

await client.api('/identityGovernance/termsOfUse/agreements')
    .version('beta')
    .post(agreement);

```