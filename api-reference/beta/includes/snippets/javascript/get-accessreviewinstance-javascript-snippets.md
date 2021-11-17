---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 846de57ba1baf13e31625fc69be687b73dd3b21f1f6df15b7817d9e7d10b1ef4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902681"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewInstance = await client.api('/identityGovernance/accessReviews/definitions/6af553ce-104d-4842-ab5f-67d7b556e9dd/instances/9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24')
    .version('beta')
    .get();

```