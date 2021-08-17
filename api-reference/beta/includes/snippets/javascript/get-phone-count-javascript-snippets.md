---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e32d33e5d87d5eda51b2d86d609b19c863b411dfc0edb3d0b06745eb08d95fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218482"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/contacts')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:wa')
    .get();

```