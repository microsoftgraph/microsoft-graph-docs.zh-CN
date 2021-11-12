---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e803d31e8ac74df3c4a02c7d6cdb01b51996302d6e9feaf50ef862f1a9625e5f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903785"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicies = await client.api('/groupLifecyclePolicies')
    .version('beta')
    .get();

```