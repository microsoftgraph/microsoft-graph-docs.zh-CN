---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85cdbee9f6c8c0d6b9bd0cd9537274183a7b587d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateProperties = {
  displayName: 'Myprefix_test_mysuffix',
  mailNickname: 'Myprefix_test_mysuffix',
  onBehalfOfUserId: 'onBehalfOfUserId-value'
};

await client.api('/groups/{id}/validateProperties')
    .post(validateProperties);

```