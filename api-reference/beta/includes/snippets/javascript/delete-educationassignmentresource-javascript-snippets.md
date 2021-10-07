---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6870176dd31fb44742bb2a64c11de83b6685e4af0eeecf4de40f0ebdd2410285
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278302"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11021/assignments/19002/resources/22002')
    .version('beta')
    .delete();

```