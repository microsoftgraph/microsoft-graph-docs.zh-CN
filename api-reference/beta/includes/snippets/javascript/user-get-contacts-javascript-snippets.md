---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7333d4b98a973f933b06865fef56e1309d3de51ac7cdce8b6e865073da7b247
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378351"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/me/contacts')
    .version('beta')
    .select('displayName,emailAddresses')
    .get();

```