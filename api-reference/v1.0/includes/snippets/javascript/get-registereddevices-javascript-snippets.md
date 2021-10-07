---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fff15c8697a2f07389043e66a358b99047eb51ac885ed524e041992c1fbf139
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registeredDevices = await client.api('/me/registeredDevices')
    .get();

```