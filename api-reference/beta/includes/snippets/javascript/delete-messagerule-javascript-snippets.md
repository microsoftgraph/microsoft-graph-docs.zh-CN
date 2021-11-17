---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ec850216c728497f8a7f83934e28ab41e219be6b9bd6d9c9be067ba2222baa3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158521"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')')
    .version('beta')
    .delete();

```