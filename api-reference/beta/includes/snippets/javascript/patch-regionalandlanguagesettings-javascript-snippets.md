---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e38d9e34a452ded41c6c037666607e4bde768475cb157ae2cb9cc4cdb9422fc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219099"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const regionalAndLanguageSettings = {
  authoringLanguages: [
    {
     locale: 'en-US' },
    {
     locale: 'es-MX' }
  ],
  defaultRegionalFormat: {
     locale: 'en-US'
   }
};

await client.api('/me/settings/regionalandlanguagesettings')
    .version('beta')
    .update(regionalAndLanguageSettings);

```