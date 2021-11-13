---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fc7cf5049f759d886db0d05e2c623a24a31adaf19a6914aaa0ddb9a5941d747
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/drive/root/delta?token=latest')
    .version('beta')
    .get();

```