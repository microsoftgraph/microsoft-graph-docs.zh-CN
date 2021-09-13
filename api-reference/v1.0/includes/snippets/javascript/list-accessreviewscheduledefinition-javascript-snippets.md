---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c931af1261d414afa0a176b7989155e317224931a0b6cd9ac3321316c2b4c9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903003"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let definitions = await client.api('/identityGovernance/accessReviews/definitions')
    .skip(0)
    .top(100)
    .get();

```