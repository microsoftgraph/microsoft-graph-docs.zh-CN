---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89bb6ca50afe3b427e44b2cb75c2d1bbbf50cdd3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865855"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive')
    .post();

```