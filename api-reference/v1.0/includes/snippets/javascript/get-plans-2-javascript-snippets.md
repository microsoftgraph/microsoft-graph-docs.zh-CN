---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 628be66082a4b06ec57e6cf5f306f5fbb6953c9871eadd191e25e163598dc2e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218698"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/groups/{group-id}/planner/plans')
    .get();

```