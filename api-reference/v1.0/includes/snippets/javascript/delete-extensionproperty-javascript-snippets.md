---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f638121b8da270bf8067e7c2f7489db9d71bc832
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999342"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/extensionProperties/{id}')
    .delete();

```