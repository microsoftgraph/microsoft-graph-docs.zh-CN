---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eca69057179282f39a528e8ecfbd390fc4cc1a74370d26d7aa45336198cfe15d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let instances = await client.api('/identityGovernance/accessReviews/definitions/2dca8959-b716-4b4c-a93d-a535c01eb6e0/instances')
    .get();

```