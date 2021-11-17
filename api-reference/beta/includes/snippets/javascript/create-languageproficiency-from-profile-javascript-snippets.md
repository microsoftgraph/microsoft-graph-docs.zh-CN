---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 188b8f4fcc59825e82439fcccda1e9cbb400ea6f934844c6769581aa59939f04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278446"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const languageProficiency = {
  displayName: 'Norwegian Bokmål',
  tag: 'nb-NO',
  spoken: 'nativeOrBilingual',
  written: 'nativeOrBilingual',
  reading: 'nativeOrBilingual'
};

await client.api('/me/profile/languages')
    .version('beta')
    .post(languageProficiency);

```