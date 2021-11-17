---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63f6d45cec63820b18d8785cadabbe50331b6eb0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "61030424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threads = await client.api('/groups/4d81ce71-486c-41e9-afc5-e41bf2d0722a/conversations/AAQkAGRhZmRhMWM3LTYwZTktNDZmYy1hNWU1LThhZWU4NzI2YTEyZgAQABKPPJ682apIiV1UFlj7XxY=/threads')
    .version('beta')
    .get();

```