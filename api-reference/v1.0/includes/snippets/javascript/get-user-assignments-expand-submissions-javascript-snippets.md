---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1ca86d7e528c1441b0c96668bb1ad68f8f3f869
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111076"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/education/users/80cefd93-8d88-40e2-b5d3-67898383e226/assignments?expand=submissions')
    .get();

```