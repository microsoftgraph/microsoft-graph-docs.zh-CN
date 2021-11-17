---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f4144237cafe1780aac6350dc5c87868c66518d379cb8e4c550f6c1a650a846
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personInterest = await client.api('/me/profile/interests/{id}')
    .version('beta')
    .get();

```