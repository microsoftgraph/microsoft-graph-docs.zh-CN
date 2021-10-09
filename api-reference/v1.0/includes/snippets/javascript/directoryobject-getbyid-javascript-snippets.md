---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3164f3684549bdb15697eb0393124132c5dbfc2aaec47c3efaf659d54c39e86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    ids: ['84b80893874940a3-97b7-68513b600544','5d6059b6368d-45f8-91e18e07d485f1d0'],
    types: ['user']
};

await client.api('/directoryObjects/getByIds')
    .post(directoryObject);

```