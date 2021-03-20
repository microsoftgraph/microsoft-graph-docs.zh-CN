---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44c5d39f36f1a5df59b3b4a019afbafe2ef151f3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942018"
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