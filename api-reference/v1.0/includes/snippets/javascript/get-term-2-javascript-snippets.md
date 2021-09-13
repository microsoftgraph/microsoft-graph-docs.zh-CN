---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fede0ca7ac2702d577aff346a46c9f7c1282a51
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/sets/17de5527-72f2-47ce-854e-99c0c5af5c17/children')
    .get();

```