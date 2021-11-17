---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ab264052f9d3d4c4f137fbbc831a17a2a986d2ebb61456309ee0bb4dd08e7bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let custodian = await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239')
    .version('beta')
    .get();

```