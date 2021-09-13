---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1116b365d57265e0a776b561ee0ef1dc8e4ae338c3c9b6401cddaaf075169ccc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332597"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connections = await client.api('/connections')
    .get();

```