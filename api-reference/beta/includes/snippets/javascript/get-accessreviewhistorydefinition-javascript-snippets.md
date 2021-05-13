---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19420915de91b80a8156fd56e4ca756c3718ef82
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474179"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewHistoryDefinition = await client.api('/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38')
    .version('beta')
    .get();

```