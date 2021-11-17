---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a864c7388f180402044888f86773f4d3e36009ba39f70d6ad70f38fc8fa8c342
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let profile = await client.api('/me/profile')
    .version('beta')
    .expand('skills($select=displayName)')
    .get();

```