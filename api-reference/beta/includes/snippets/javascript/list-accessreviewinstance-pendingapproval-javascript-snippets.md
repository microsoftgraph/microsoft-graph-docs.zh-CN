---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4763706e2179870bcb071c201faa01fe1edf3385ab3ed0d3e02e361af2d7eef7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104140"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let pendingAccessReviewInstances = await client.api('/me/pendingAccessReviewInstances')
    .version('beta')
    .expand('definition')
    .skip(0)
    .top(100)
    .get();

```