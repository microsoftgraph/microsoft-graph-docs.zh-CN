---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: d31350200e7b6d999e52e740306c6df9688bb4e9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/accessReviews/definitions/29f2d16e-9ca6-4052-bbfe-802c48981fd8')
    .version('beta')
    .delete();

```