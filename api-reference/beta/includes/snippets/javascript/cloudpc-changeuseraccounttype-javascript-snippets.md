---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8f627eb506f92f3aa560bfd8d0e87841604cd49
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const changeUserAccountType = {
  userAccountType: 'administrator'
};

await client.api('/deviceManagement/virtualEndpoint/cloudPCs/4b5ad5e0-6a0b-4ffc-818d-36bb23cf4dbd/changeUserAccountType')
    .version('beta')
    .post(changeUserAccountType);

```