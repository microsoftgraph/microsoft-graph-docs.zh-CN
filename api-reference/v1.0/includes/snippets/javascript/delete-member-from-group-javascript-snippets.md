---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe981446dd87c574b931154b80204f0a365533dc037928810992c7cfbc5c78d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{group-id}/members/{directory-object-id}/$ref')
    .delete();

```