---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01126ca2fc43f4ce52225fe1d81c34daa4c2306a
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573133"
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