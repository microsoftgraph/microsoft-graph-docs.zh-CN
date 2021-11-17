---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6712b4a7a411cc3cc6eb27e2876219755d3c4520b06f68bbfef198e21d48093f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158616"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReview = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d')
    .version('beta')
    .get();

```