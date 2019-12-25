---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35ffd786c3cb5798c2052d1b0f9eeca2326d90d9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscribeToToneOperation = {
  clientContext: "fd1c7836-4d84-4e24-b6aa-23188688cc54"
};

let res = await client.api('/communications/calls/{id}/subscribeToTone')
    .post(subscribeToToneOperation);

```