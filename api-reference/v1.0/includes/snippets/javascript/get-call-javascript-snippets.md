---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8119561aae18de9c92720709c67cb6cf4da803f9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871119"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92')
    .get();

```