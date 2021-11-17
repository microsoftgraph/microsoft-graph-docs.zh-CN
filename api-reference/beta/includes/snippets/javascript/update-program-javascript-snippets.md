---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9066decfbd6786d41548a2ea70be7c390492024519c0d1e24421b4ae1892362c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const program = {
    displayName: 'testprogram3 new name'
};

await client.api('/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
    .version('beta')
    .update(program);

```