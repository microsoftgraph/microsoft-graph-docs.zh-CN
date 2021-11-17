---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19a52b3bde2640d787bee14837612d06fb6136788182784bf25496ec79d09f03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277468"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userSource = await client.api('/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735')
    .version('beta')
    .get();

```