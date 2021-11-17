---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a9eaa562299d2908c09b4d29bf828944adc7f93baab1b41e214dd2ba372cfd2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273845"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let interests = await client.api('/me/profile/interests')
    .version('beta')
    .get();

```