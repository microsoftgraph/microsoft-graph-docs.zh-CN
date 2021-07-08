---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c139df6e3c39b18a209664fad0e290002a8f9c0
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53319577"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let decisions = await client.api('/identityGovernance/accessReviews/definitions/2dca8959-b716-4b4c-a93d-a535c01eb6e0/instances/8d035c9d-798d-47fa-beb4-f986a4b8126f/decisions')
    .get();

```