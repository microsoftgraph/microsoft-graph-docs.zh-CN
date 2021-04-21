---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cc3389554b7c96c59d35205c9fdcebe0bcbf009
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920071"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    pkcs12Value: 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA',
    password: '<password>'
};

await client.api('/identity/apiconnectors/{id}/uploadClientCertificate')
    .version('beta')
    .post(identityApiConnector);

```