---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae19850bf86d20150178be891f6c0b1a7a694218
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474158"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let historyDefinitions = await client.api('/identityGovernance/accessReviews/historyDefinitions')
    .version('beta')
    .get();

```