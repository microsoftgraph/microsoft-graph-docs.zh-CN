---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 535e0b9a422c4c3c7db4466b4fbe4808ff4e95dca1b5e8f345255f0792a4f0bb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104605"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/drive/root/delta')
    .get();

```