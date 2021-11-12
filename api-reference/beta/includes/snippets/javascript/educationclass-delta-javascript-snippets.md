---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05bd48e16826a150006f0d2c99460db220e41964bca5d59538f9893ec3b48e18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/classes/delta')
    .version('beta')
    .get();

```