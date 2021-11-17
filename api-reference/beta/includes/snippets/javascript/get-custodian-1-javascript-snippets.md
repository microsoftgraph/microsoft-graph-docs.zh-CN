---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff482d366dab454987d1d066979356826bbaa6cc7380b87117f8baa7e70199d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let custodians = await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians')
    .version('beta')
    .get();

```