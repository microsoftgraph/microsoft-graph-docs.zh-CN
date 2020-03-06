---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16732b42e16ee2a46fb1e446255dc2ef39248f0b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37999469"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removePassword = {
    keyId: "f0b0b335-1d71-4883-8f98-567911bfdca6"
};

let res = await client.api('/applications/{id}/removePassword')
    .post(removePassword);

```