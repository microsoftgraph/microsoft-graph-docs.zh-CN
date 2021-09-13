---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 622970ce1dd6d8196150ea4f4a9474ff465659dfbf719bd0e0fc60d09f14d210
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904089"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffReasons = await client.api('/teams/{teamId}/schedule/timeOffReasons')
    .get();

```