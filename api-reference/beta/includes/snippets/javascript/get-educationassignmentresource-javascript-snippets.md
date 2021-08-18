---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66138ce31ead72c0962bceb8957e8fb8c89f62ff49dfccf28d29c33e3ea8eeb1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentResource = await client.api('/education/classes/11021/assignments/19002/resources/22002')
    .version('beta')
    .get();

```