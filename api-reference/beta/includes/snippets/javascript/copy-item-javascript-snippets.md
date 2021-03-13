---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfc7a0a727e2330c8de3aa4fd05137ed9882469e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    driveId: '6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B',
    id: 'DCD0D3AD-8989-4F23-A5A2-2C086050513F'
  },
  name: 'contoso plan (copy).txt'
};

await client.api('/me/drive/items/{item-id}/copy')
    .version('beta')
    .post(driveItem);

```