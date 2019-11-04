---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcbad503ec8bc7f2881a7688805e26ecf4919265
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937506"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  key: "key-value"
};

let res = await client.api('/trustFramework/keySets/{id}/uploadCertificate')
    .version('beta')
    .post(trustFrameworkKey);

```