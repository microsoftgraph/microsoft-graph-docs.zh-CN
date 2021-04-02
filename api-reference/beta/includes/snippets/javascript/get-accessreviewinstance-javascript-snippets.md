---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa1f92b750a499983e3e6eeff544a10b95b17725
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507209"
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