---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d53556ed95ab4e25803acbbfe3cb1830c4d18dad8bb534c387bd4a090cadd0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902643"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewPolicy = {
  isGroupOwnerManagementEnabled: true
};

await client.api('/identityGovernance/accessReviews/policy')
    .version('beta')
    .update(accessReviewPolicy);

```