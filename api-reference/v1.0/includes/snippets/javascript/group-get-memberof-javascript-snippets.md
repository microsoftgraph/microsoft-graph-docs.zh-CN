---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f09f3d6ec2a3e483c9cf37707c922aaba660049057277363477524e637fd0e72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106737"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/groups/{id}/memberOf')
    .get();

```