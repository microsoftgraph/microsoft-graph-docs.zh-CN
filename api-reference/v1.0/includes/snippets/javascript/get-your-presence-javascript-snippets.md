---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fb1792e081a091dd2b5fd7e3382f6ed45a0797d36c395ce00eea4e1aada112b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let presence = await client.api('/me/presence')
    .get();

```