---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b19241384869cdb2181c774fb633869612bed5c
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setVerifiedPublisher = {
    verifiedPublisherId: "1234567"
};

let res = await client.api('/applications/{id}/setVerifiedPublisher')
    .post(setVerifiedPublisher);

```