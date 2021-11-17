---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc6daccb8603bc43eba34927c88cbf87e9721508bac5916570d2b5a9d356990b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277384"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let usageRights = await client.api('/users/{userId}/usageRights')
    .version('beta')
    .filter('state in (\'active\', \'suspended\') and serviceIdentifier in (\'ABCD\')')
    .get();

```