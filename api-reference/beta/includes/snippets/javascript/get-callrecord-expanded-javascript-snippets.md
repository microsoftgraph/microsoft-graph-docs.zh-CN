---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd4335f83efc05d93aa695c1d1264935f0c559bc01d23710da623772e1b6cab4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105655"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let callRecord = await client.api('/communications/callRecords/{id}')
    .version('beta')
    .expand('sessions($expand=segments)')
    .get();

```