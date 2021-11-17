---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41b38e57eb91fe88aed91fb479521d334f7c56849db3a12be4d9f5b2195f65e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/unsetVerifiedPublisher')
    .version('beta')
    .post();

```