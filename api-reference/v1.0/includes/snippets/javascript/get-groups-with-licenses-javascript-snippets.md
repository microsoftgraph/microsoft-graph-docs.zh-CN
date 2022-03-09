---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd0ba9a91e1c4d5d641db8cbe80cfaf784219b3b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393632"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/groups')
    .filter('assignedLicenses/any()')
    .select('id,assignedLicenses')
    .get();

```