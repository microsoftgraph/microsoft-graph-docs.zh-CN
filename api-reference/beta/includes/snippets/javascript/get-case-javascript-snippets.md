---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d53c3d1de1a00c477a147d5ef0d7dac110e468ce093b32255c426c29a10ee5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let _case = await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583')
    .version('beta')
    .get();

```