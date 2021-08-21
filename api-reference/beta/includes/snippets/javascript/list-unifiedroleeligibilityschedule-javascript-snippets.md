---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e79cdd403cad8863b8abd069f7dc603e23553b58f82b17288b6183aa34eba9e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleEligibilitySchedules = await client.api('/roleManagement/directory/roleEligibilitySchedules')
    .version('beta')
    .get();

```