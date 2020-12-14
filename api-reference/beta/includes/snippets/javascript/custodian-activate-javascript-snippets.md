---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28a74e4a17f297297b288ce87cc43cc5802fe118
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/activate')
    .version('beta')
    .post();

```