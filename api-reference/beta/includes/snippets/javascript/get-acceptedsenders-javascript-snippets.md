---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e37855b3f67d7742f89426c3ae024fd0cbed1ebf0854b275d52f82942b958c7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let acceptedSenders = await client.api('/groups/{id}/acceptedSenders')
    .version('beta')
    .get();

```