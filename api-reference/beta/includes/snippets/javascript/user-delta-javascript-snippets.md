---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab41ba53297f248dc1bbd36cbe9cef21ff559bf87baf6222babebbbe0f34951f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158342"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/users/delta')
    .version('beta')
    .get();

```