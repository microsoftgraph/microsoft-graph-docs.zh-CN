---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2722eb450c9d40fc7b5fc1b66f6e3db71517a0c5
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933807"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/unfollow')
    .version('beta')
    .delete();

```