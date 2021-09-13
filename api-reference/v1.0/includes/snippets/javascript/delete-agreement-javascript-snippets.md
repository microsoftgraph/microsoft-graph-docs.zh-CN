---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08536e3d4057e491ca4e0294de4d25fcc6a30c0bae8cc58e6e57a4ba0545ab4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be')
    .delete();

```