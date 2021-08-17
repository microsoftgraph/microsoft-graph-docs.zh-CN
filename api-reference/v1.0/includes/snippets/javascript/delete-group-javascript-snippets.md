---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6143ad908f98be2a05e957051953d215362449b90b2bbfeef659582abb81773a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}')
    .delete();

```