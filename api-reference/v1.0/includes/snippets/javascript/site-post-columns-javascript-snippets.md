---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c030760423deb74cf7ffc297b5feab8851e8c083
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const columnDefinition = {
   description: 'test',
   enforceUniqueValues: false,
   hidden: false,
   indexed: false,
   name: 'Title',
   text: {
      allowMultipleLines: false,
      appendChangesToExistingText: false,
      linesForEditing: 0,
      maxLength: 255
   }
};

await client.api('/sites/{site-id}/columns')
    .post(columnDefinition);

```