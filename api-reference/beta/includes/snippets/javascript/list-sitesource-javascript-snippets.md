---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c503cae00ca6fe15bceb8f5cfed078acdcc32a70
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773072"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let siteSources = await client.api('/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/siteSources')
    .version('beta')
    .get();

```