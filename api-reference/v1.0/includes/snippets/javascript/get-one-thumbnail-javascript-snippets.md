---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83680eb143d7e7237681f31ab60c0569f38f1cbd6f68f0782a16c160348fff27
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378461"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let response = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}')
    .get();

```