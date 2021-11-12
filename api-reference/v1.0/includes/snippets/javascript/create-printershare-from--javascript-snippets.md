---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e8388cdde07823c096158cc229c7e670e219b8ba6adc0f730fb2a51d3b69dac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printerShare = {
  displayName: 'ShareName',
  allowAllUsers: false,
  'printer@odata.bind': 'https://graph.microsoft.com/v1.0/print/printers/{printerId}'
};

await client.api('/print/shares')
    .post(printerShare);

```