---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b421662145e11c1ecf59f0104b0f57de97431f7c8ee2d9d10c907640ae5e7d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332172"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/resetDecisions')
    .post();

```