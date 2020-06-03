---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bfcca9ce24f43e915e9cc43e42e151325c879a2
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/callRecords/{id}')
    .version('beta')
    .get();

```