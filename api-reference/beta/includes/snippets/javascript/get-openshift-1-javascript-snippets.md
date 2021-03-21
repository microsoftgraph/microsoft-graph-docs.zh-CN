---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea2eebf3dd93e9389bb4b7d1d6001db4a12cafec
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954440"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShift = await client.api('/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8')
    .version('beta')
    .get();

```