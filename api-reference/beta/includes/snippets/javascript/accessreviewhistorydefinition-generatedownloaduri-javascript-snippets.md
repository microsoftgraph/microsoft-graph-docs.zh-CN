---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a400adcd16ce63b385f1ef82934d2de012f9cc7481e22bd91f9148f01f78344
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/accessReviews/historyDefinitions/b2cb022f-b7e1-40f3-9854-c65a40861c38/generateDownloadUri')
    .version('beta')
    .post();

```