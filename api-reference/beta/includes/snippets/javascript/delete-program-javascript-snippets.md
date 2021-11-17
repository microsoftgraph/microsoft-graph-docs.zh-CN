---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 878b744e986d2b9a4cb22530ee0c1f53b2e446733093269c1813e93edf9f0dbb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162456"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
    .version('beta')
    .delete();

```