---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d923171853dc7e9e657720eb1ad54400b639db65486db48251d1c67d654456a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409658"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .get();

```