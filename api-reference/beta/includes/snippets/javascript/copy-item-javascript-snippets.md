---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50e6cd143bd3561be204b1641969e80fac2e6905c94a48fa8ed6f590d9a6dc32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332407"
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