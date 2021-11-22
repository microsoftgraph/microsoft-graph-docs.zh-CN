---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 138d292492ff3cbc803a9b53b90fdfe833fbc5482f879a8912abacd7495773a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274354"
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