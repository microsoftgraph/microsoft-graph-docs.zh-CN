---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e366c84108a415b4e55cf66c98b18ea7ab7e04d4
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524617"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/callRecords/{id}')
    .expand('sessions($expand=segments)')
    .get();

```