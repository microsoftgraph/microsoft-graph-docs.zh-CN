---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e402a2b036a4ed908479b3100dd1dcf3a8598363
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setVerifiedPublisher = {
    verifiedPublisherId: '1234567'
};

await client.api('/applications/{id}/setVerifiedPublisher')
    .version('beta')
    .post(setVerifiedPublisher);

```