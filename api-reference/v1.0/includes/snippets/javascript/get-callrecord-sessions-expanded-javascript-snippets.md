---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eee286e7ef61c26aa364796f024a22106b468f782cbe2e86ce6f6781b898a700
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279387"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sessions = await client.api('/communications/callRecords/{id}/sessions')
    .expand('segments')
    .get();

```