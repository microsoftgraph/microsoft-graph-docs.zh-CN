---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 404eb3c1cef6010b11dc43115e88881460212d73fcef94d68c3a4099fe7c69eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const copyToDefaultContentLocation = {
   sourceFile: {
      sharepointIds: {
         listId: 'e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0',
         listItemId: '2'
      }
   },
   destinationFileName: 'newname.txt'
};

await client.api('/sites/{id}/contentTypes/{contentTypeId}/copyToDefaultContentLocation')
    .version('beta')
    .post(copyToDefaultContentLocation);

```