---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a982fedfa83633ac1059cc6e5fb74117b13a5be76debb0969ad089c37f9256d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161291"
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