---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fca835c16fc657fe0c6cd06b5efbb7d4acf2b2f
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39640413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
    displayName: "Seattle District Technical Schools",
    description: "Seattle district technical schools administration",
    visibility: "HiddenMembership"
};

let res = await client.api('/administrativeUnits')
    .version('beta')
    .post(administrativeUnit);

```