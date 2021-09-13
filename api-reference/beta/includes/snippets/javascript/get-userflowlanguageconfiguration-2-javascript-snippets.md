---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a705b94187edbc2f1b27015b57f6a390ca74e81a485dc599dd8ac72c921f28a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105657"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let languages = await client.api('/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages')
    .version('beta')
    .get();

```