---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b859751d97e8c9d8151da2f003d1656f87c9f156fea4ad95c5246087f5af0ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/me/getMemberObjects')
    .version('beta')
    .post(string);

```