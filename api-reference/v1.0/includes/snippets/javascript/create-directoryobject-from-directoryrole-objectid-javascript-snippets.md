---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc2483a249cd854fc708336ccde1e19c96c0ced6
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "53005834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/15c1a2d5-9101-44b2-83ab-885db8a647ca'
};

await client.api('/directoryRoles/fe8f10bf-c9c2-47eb-95cb-c26cc85f1830/members/$ref')
    .post(directoryObject);

```