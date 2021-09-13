---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91ec031d9971fcf97fbd2fb132b2009ea14baf11
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025712"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let relations = await client.api('/sites/microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74/termStore/sets/874be29c-35c8-4295-b3f8-ca2400c966c3/relations')
    .get();

```