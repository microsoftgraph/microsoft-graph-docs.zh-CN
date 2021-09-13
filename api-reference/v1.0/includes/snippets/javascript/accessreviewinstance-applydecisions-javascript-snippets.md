---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 673dd2170ec9c0876d5f5f5514c144bafe17ef3d03b541d3105e0251750e984e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105441"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-5678-8868-0810c7f49101/applyDecisions')
    .post();

```