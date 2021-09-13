---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8e95735a85c5a85b2cab4fb71b54e17807cf4258c2ae77c90a05627665acf72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewInstance = await client.api('/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/12345ba0-cbf0-5678-8868-4444c7f4cc06')
    .get();

```