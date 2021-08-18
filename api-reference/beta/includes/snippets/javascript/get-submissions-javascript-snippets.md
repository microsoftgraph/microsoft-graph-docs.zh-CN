---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c4b8418c425b198304a1f19f23dad93368e5236601ea3fbf9bef4a1b95d1048
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let submissions = await client.api('/education/classes/11021/assignments/19002/submissions')
    .version('beta')
    .get();

```