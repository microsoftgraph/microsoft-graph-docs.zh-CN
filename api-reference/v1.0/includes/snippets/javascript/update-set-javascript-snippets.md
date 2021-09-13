---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 797d0ad8a006e822d5454f2e3f2c28e024cf57c7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const set = {
  description: 'mySet'
};

await client.api('/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/sets/3607e9f9-e9f9-3607-f9e9-0736f9e90736')
    .update(set);

```