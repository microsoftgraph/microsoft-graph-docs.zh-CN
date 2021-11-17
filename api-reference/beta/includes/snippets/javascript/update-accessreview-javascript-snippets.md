---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5db5566410120628d7388adbbba8a591d1cd1e4e18ce53ed060a61168e49b0f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902706"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReview = {
    displayName: 'TestReview new name'
};

await client.api('/accessReviews/006111db-0810-4494-a6df-904d368bd81b')
    .version('beta')
    .update(accessReview);

```