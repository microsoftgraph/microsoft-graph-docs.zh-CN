---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9307f4785b958fe7c7fad252a6678a2591d4c27
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60718093"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const term = {
  labels: [
    {
      languageTag: 'en-US',
      name: 'Car',
      isDefault: true
    }
  ]
};

await client.api('/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/sets/462bd0ae-30bb-4c58-845c-761ff6481ac1/children')
    .post(term);

```