---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76084ca1c65c19622232a69243eac79f7f410df23bbc03c9ba7460df493f04c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4')
    .version('beta')
    .get();

```