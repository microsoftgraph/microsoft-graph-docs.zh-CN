---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b053761b988e867def6d9e30aae22feba273e190
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932667"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/bundles/{bundle-id}')
    .version('beta')
    .get();

```