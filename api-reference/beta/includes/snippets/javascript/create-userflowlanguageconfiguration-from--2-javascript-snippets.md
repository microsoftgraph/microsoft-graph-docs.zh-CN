---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77146854d975920609cfb5ca0fd9432522d12b0d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944634"
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