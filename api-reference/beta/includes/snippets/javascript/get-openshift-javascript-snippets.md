---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13e2d4f67ae4395857e5a05cfef52e76a24e121b
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945304"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8')
    .version('beta')
    .get();

```