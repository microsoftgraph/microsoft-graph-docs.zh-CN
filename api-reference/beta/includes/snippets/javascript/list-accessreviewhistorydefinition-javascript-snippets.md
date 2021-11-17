---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3714a1fb65a68de1519a888615f49141f5b0d928f4bff2e7eea35f7354538030
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104150"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let historyDefinitions = await client.api('/identityGovernance/accessReviews/historyDefinitions')
    .version('beta')
    .get();

```