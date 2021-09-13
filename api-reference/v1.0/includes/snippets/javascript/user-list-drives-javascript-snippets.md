---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87d9c6e6ea2af5df41bd87a5d5dbefb8913b69886295b6c568085e5994194bad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218417"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/users/{userId}/drives')
    .get();

```