---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 328d76f9ffd8818f9c50d3ca1f2bce9a28621622a9a16297767f70501cfa8d73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333491"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicy = await client.api('/groupLifecyclePolicies/{id}')
    .get();

```