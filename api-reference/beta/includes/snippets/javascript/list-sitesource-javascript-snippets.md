---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61b96e1e8a7802ec689bc8ae2cb30a70ff8ac163
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502955"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let siteSources = await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/siteSources')
    .version('beta')
    .get();

```