---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b95a9b86cedc80cae51cb01522f7be4d9b608ee39b413a9bdad100dfaf1046f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333980"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extensionProperty = {
  isSyncedFromOnPremises: 'Boolean'
};

await client.api('/directoryObjects/getAvailableExtensionProperties')
    .post(extensionProperty);

```