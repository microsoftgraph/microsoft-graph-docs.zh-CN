---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59b964d348d94403c47c1ee1914ef76c64ac165b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772525"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let asHierarchy = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/asHierarchy')
    .version('beta')
    .get();

```