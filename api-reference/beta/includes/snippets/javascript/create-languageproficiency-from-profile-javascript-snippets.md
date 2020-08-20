---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d77a9851c741112f49e7b21b1d3e93d94e8745e8
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821096"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const languageProficiency = {
  displayName: "Norwegian Bokmål",
  tag: "nb-NO",
  spoken: "nativeOrBilingual",
  written: "nativeOrBilingual",
  reading: "nativeOrBilingual"
};

let res = await client.api('/me/profile/languages')
    .version('beta')
    .post(languageProficiency);

```