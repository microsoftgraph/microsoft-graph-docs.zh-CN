---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4947b9188e2b1cbaba04afc8e720ff4354a2d91a3f7ab645adffd83bdc50d643
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104609"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateProperties = {
  entityType: 'Group',
  displayName: 'Myprefix_test_mysuffix',
  mailNickname: 'Myprefix_test_mysuffix',
  onBehalfOfUserId: 'onBehalfOfUserId-value'
};

await client.api('/directoryObjects/validateProperties')
    .post(validateProperties);

```