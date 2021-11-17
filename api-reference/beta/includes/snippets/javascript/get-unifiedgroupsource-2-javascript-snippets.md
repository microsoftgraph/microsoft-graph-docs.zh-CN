---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f409b9129884e186010e6de77f19e15e8e6ed442ec7b5ba5b53930374d8b8fe2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218562"
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