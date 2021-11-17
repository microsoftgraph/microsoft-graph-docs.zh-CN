---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aaf98edf9ec10a30c9e78e93f40023d7837ca78d0e39bf6c17ca88db6ec084f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreement = await client.api('/identityGovernance/termsOfUse/agreements/{id}')
    .version('beta')
    .expand('files')
    .get();

```