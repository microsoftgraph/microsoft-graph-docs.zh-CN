---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 991b3609039842253323778e1c93bfea6e22a332e9736d2808a7c0cc2b661889
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162499"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let addToReviewSetOperation = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119/addToReviewSetOperation')
    .version('beta')
    .get();

```