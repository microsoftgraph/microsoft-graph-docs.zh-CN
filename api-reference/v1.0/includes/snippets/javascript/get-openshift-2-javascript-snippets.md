---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 136b5a10806afe6f03624d22a8d91d813242590bdf68286fdd972ff6839ade4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162566"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShifts = await client.api('/teams/{id}/schedule/openShifts')
    .get();

```