---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbd8702c349230025bf941454828574d05a4a09b17943730a3cb3aec45973d5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219096"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getCredentialUsageSummary = await client.api('/reports/getCredentialUsageSummary(period='D30')')
    .version('beta')
    .filter('feature eq \'registration\'')
    .get();

```