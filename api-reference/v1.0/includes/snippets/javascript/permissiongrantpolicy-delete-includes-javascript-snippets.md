---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7b3d1bf118c9b7d411183e357a2ad5d99840ce9365690827da9dd0c762eddd2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274224"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5')
    .delete();

```