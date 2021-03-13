---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e85500c577d24e42d9acee9ff5cd05a16568fb8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801261"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735')
    .version('beta')
    .delete();

```