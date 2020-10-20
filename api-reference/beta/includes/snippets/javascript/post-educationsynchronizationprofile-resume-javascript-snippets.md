---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba09b907027808a91b2823c030c7cc8fec942502
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616180"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/resume')
    .version('beta')
    .post();

```