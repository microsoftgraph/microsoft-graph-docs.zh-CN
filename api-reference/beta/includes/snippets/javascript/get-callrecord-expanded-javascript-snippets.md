---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e19a2c13595d5e05d394bf9476d1619ccaa9e4e9
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/callRecords/{id}')
    .version('beta')
    .expand('sessions($expand=segments)')
    .get();

```