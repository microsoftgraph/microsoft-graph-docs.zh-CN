---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b94a60c1dcd5d7a9e13ab74159485cf71d9879e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393534"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupSetting = await client.api('/groupSettings/84af2ca5-c274-41bf-86e4-6e374ec4def6')
    .get();

```