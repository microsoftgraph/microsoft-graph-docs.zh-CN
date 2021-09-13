---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c789673dd976f9f3dde228cb9b3070de9cc2d1bb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147629"
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

await client.api('/sites/{siteId}/contentTypes/{contentTypeId}/copyToDefaultContentLocation')
    .post(copyToDefaultContentLocation);

```