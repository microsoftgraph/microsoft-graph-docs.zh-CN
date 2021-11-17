---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2345462568cc7d00084177be1c6d4bb4e9ce023c9ad4ff8f2e57d7929d7ee108
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158344"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/users/delta')
    .version('beta')
    .select('displayName,jobTitle,mobilePhone')
    .get();

```