---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ab8c8347be8b4860459bd3daf745c7fe46e1fd7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777164"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printerShare = {
  displayName: 'ShareName',
  allowAllUsers: false,
  'printer@odata.bind': 'https://graph.microsoft.com/v1.0/print/printers/{printerId}'
};

await client.api('/print/shares')
    .post(printerShare);

```