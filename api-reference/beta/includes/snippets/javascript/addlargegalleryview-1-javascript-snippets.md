---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2f8443f22f45fd6d3916e4214ca623819207d43
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addLargeGalleryViewOperation = {
  clientContext: '785f4929-92ca-497b-863f-c778c77c9758'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/addLargeGalleryView')
    .version('beta')
    .post(addLargeGalleryViewOperation);

```