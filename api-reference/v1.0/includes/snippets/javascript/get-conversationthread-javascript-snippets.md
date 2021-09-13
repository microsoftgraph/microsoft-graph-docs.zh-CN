---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 930cca70df160daa391ad7c84db2f4141d279f61e750d63497003ff1c2d96db9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331843"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversationThread = await client.api('/groups/{id}/threads/{id}')
    .get();

```