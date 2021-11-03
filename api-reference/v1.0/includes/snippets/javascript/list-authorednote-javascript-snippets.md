---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80153581c752dfdfebf28b39405f0c86fc6c5c1d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687906"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notes = await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes')
    .get();

```