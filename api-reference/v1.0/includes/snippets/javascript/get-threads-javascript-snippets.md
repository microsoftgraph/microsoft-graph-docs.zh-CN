---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 707b98341c0593431bb587c0e7391972477c161c41663adc24579f8e788ee8af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107086"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threads = await client.api('/groups/{id}/conversations/{id}/threads')
    .get();

```