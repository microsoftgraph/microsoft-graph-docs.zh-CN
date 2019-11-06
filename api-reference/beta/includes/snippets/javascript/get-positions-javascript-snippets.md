---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef5d21524fe67baca6b402e77e90d9c5cfed49b1
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997926"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/positions')
    .version('beta')
    .get();

```