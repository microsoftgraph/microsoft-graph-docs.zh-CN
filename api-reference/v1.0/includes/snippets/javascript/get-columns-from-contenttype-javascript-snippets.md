---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3914603d6186fc7616a43a78fd553cabea032ec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038232"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/sites/{site-id}/contentTypes/{contentType-id}/columns')
    .get();

```