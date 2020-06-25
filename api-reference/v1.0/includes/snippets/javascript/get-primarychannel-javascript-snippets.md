---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4b411e54a425d1a1c0071b531ee79359a2a9fd7
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863891"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/primaryChannel')
    .get();

```