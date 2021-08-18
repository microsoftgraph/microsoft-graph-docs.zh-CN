---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7e1fb8cbfcc875d789395d2d8fc5d262b1735ee98de923ca016c4ae77165aae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220688"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSubmissionResource = await client.api('/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024')
    .version('beta')
    .get();

```