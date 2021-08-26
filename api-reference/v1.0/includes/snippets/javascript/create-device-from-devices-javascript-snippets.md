---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07c2a43ec027dd11ae5048abc9e1e6269a628be53b570b8f68cccf96ffb9767d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333524"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled: false,
  alternativeSecurityIds: 
  [
    {
      type: 2,
      key: 'base64Y3YxN2E1MWFlYw=='
    }
  ],
  deviceId: '4c299165-6e8f-4b45-a5ba-c5d250a707ff',
  displayName: 'Test device',
  operatingSystem: 'linux',
  operatingSystemVersion: '1'
};

await client.api('/devices')
    .post(device);

```