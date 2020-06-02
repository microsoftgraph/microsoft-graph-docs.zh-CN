---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: beb90e11f48b6a0aeb31de5afac40d75805f478f
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44219212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8')
    .version('beta')
    .delete();

```