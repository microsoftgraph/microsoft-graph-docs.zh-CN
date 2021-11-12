---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 124aa025a14700878df6d6d18f516793e55da4e09084fa49a6fe859823d3701b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328698"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroups = await client.api('/me/onenote/sectionGroups')
    .version('beta')
    .get();

```