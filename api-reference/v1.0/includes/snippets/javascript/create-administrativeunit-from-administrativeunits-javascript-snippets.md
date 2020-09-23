---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78089053c41ae072da631fc6d36c0ebd04cf9612
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223614"
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

let res = await client.api('/directory/administrativeUnits')
    .post(administrativeUnit);

```