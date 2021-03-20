---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e32e26c82972023a361312c51e8ebe11b433adb5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951896"
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