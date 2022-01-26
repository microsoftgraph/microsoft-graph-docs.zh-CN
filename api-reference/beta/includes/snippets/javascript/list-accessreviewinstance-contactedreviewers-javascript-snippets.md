---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 743b1fe9ae5ffbf8b76ea84076c66df7d95fab9b
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225175"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contactedReviewers = await client.api('/identityGovernance/accessReviews/definitions/2dca8959-b716-4b4c-a93d-a535c01eb6e0/instances/8d035c9d-798d-47fa-beb4-f986a4b8126f/contactedReviewers')
    .version('beta')
    .get();

```