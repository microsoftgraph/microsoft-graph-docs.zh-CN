---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba9ea9ec97193404e4269f23220c3abeda2b8574d3980fee3d32b0365431cf25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
    .delete();

```