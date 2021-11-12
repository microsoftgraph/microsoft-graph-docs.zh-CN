---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8f3e0dbc918488fef90173bfee638272522513310ae4dfc0fa3d57062d80b51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378575"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffReason = await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .version('beta')
    .get();

```