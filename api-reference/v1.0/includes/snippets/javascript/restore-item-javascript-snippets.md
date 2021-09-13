---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 483a168b6a00f95e93eda816fb857c1a5f6b17bb0cc695083bf200a2c99f020d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    id: 'String',
  },
  name: 'String'
};

await client.api('/me/drive/items/{item-id}/restore')
    .version('beta')
    .post(driveItem);

```