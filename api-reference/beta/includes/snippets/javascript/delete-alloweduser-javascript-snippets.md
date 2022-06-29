---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a090c65d55be6feb4b17c7dca733bd83421c8c5c00a5bd726de80d91f2d52e22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printerShares/{id}/allowedUsers/{id}/$ref')
    .version('beta')
    .delete();

```