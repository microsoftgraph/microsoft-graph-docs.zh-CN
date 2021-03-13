---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4443f337288bbd6701f18ec2886d28537bab4a5f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773737"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _case = {
    displayName: 'My Case 1',
};

await client.api('/compliance/ediscovery/cases')
    .version('beta')
    .post(_case);

```