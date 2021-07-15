---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b7107dd2fcc5f17d00217474993cbb941c806f9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440978"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let includedGroups = await client.api('/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups')
    .version('beta')
    .get();

```