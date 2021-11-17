---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c2e7d810b0b6e3e4df4cb14b8990997d6cb8c780c6e990ade2b3b1515284ec3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104128"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let decisions = await client.api('/identityGovernance/accessReviews/definitions/16d424f6-0100-4bf1-9ebc-fe009c5e5006/instances/bb14c722-51b8-4962-9bd2-1d96ba773d80/decisions')
    .version('beta')
    .get();

```