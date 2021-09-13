---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a095d38127b241c8e5cd61522dc820d2e3b0a4b2cbe297c562f317858fdde39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333519"
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
    .post(driveItem);

```