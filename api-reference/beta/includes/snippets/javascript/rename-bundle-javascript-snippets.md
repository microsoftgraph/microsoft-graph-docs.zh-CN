---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a29cafdb5e6029fde59594623b9c0dbdb0bce7099bb9c7b940411b5251bd47d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105819"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: 'Shared legal agreements'
};

await client.api('/drive/items/{bundle-id}')
    .version('beta')
    .update(driveItem);

```