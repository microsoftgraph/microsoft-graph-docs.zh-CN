---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46a671c5960fe097b66288ae461c19355d74617cb56fce442fe2942a4958dfa7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903321"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemPhone = {
  type: 'other'
};

await client.api('/users/{userId}/profile/phones/{id}')
    .version('beta')
    .update(itemPhone);

```