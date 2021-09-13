---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 558ef3c43f15d3026783e76654869d431a86783ca39e195f86e855c616651bd9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274427"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffReason = await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .get();

```