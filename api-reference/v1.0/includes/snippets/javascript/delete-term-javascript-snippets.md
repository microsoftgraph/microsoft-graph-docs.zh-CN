---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e610172179b2e17b7a338d44c54769123662a6cd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021899"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/sets/584b2331-f5c9-4b45-a5ec-d3cb9af67006/terms/a929ae3c-a11f-447f-9835-f09b461cd59a')
    .delete();

```