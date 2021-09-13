---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52db6fd8d7d55f14fc155f26aca5ba629a72508b5cf3604df61e7413b4828771
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicies = await client.api('/groupLifecyclePolicies')
    .get();

```