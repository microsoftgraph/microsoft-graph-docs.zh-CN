---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e6369b49fe485b6d9635f507f2ecfb49aeec39b4d99c96d1fc784e56fd06f6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896')
    .delete();

```