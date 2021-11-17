---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ed1692bf6fcb8bd9bbe5053d0edaac4efcf33efddd88cdec97f2ecad43459a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106352"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/activate')
    .version('beta')
    .post();

```