---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ab7cc87e6a7fa8200aceab4b9be434fd891e4b4517e083798be35ff613367e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignments = await client.api('/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments')
    .get();

```