---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9976db71f4d1cd815f1d4d751a3f6ee1a4b1cae8e9e1362a46f254c38dbfb2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groupLifecyclePolicies/{id}')
    .version('beta')
    .delete();

```