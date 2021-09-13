---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3dfd1f9884e7a4bafde2fa6d73867e398f9e80724210626abac59f8670d5695
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105576"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/me/drive/root/children')
    .get();

```