---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f90a15cd9f1870206753d4e2245cc10607e4db63249848a172f326f41debcce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userFlowLanguageConfiguration = {
  isEnabled: false
};

await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES')
    .version('beta')
    .put(userFlowLanguageConfiguration);

```