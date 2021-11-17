---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05c70db81acb1aa626fe8e479ae51822d64dce78bcba9aa97ec2f9e066703f51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/phones/{itemPhoneId}')
    .version('beta')
    .delete();

```