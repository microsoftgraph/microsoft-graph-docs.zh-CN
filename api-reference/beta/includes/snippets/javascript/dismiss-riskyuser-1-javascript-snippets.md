---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6075e4ad7090dc305ae50056e18755916583062c57cbd9c29a7b5015037e9ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903077"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dismiss = {
  userIds: [
    '04487ee0-f4f6-4e7f-8999-facc5a30e232',
    '13387ee0-f4f6-4e7f-8999-facc5120e345'
  ]
};

await client.api('/riskyUsers/dismiss')
    .version('beta')
    .post(dismiss);

```