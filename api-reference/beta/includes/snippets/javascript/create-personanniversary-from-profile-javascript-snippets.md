---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8db2a787e13f8f2c306588076d2639580c8c70891443971b453a28deee7bfde4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279491"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnualEvent = {
  type: 'birthday',
  date: '1980-01-08'
};

await client.api('/me/profile/anniversaries')
    .version('beta')
    .post(personAnnualEvent);

```