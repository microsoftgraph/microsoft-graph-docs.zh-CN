---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89f5dd81ac1443875ee2d3f922666c7cba69216d18ddd5abade7fcdbbe4636bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162255"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11021/assignments/19002/submissions/850f51b7/return')
    .version('beta')
    .post();

```