---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fb68716bee2bf8f4e2baaa902bea159510d659b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/fd918e4b-c821-4efb-b50a-5eddd23afc6f/extensionProperties/1f0f15e3-925d-40f0-8fc8-9d3ad135bce0')
    .version('beta')
    .delete();

```