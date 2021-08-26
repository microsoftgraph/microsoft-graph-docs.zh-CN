---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6f9d7eec118c4a6c14de3265d0e8fc0a39e6e14509f9b0900a90ef78689ad71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219978"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}/registeredUsers/{id}/$ref')
    .version('beta')
    .delete();

```