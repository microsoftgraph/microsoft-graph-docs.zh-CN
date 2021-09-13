---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9dacfd8edb6e6f5f48f4911a79bebffe6dd07f0d3b34a76d674f8184fcb6f906
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shift = await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .get();

```