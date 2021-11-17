---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 195ff3eec14d7bacef4a6ff5c25e81bb32bb429608937314bb0ede4e4949f4cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104032"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenIssuancePolicies = await client.api('/applications/{id}/tokenIssuancePolicies')
    .version('beta')
    .get();

```