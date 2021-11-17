---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f743a3ab8f9dd961ea721abe6c215cb6747580d4dcb5fe55533ee45aacfa5ce2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902593"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let adminConsentRequestPolicy = await client.api('/policies/adminConsentRequestPolicy')
    .version('beta')
    .get();

```