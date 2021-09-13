---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d25c5f3d3fc73f7bf3cc02ab159bd57d24b81e6fcb9ef79e08a24bf66b40711d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreement = await client.api('/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be')
    .expand('files')
    .get();

```