---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f551f068ba4f3445e18b468606febc52579a488
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951953"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedGroupSource = await client.api('/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources/33434233-3030-3739-3043-393039324633')
    .version('beta')
    .get();

```